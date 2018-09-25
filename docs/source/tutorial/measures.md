# Measures

A novelty in jMetal 5.0 is the inclusion of measures, which allows to obtain algorithm-specific information during its execution. The current implementation supports two types of measures: a `PullMeasure` provides the value of the measure on demand (synchronous), while a `PushMeasure` allows to register listeners (or observers) to receive the value of the measure when it is produced (asynchronous).

## What are measures?

Measures are designed to access specific properties of a running algorithm. For instance, one could know the size of the current population in a genetic algorithm, the current velocity of the particles in a particle swarm optimization, the current iteration, etc. In order to deal properly with the many properties that an algorithm could have, two types of measures are provided.

Usually, properties are accessed by getters, like `getPopulationSize()` or `getCurrentIteration()`. These properties are accessed in a synchronous way, which means that we obtain (and process) them on the user's demand. Each property of this kind can be accessed through a `PullMeasure`, as shows the `PullMeasure.get()` method:
```
public interface PullMeasure<Value> extends Measure<Value> {
	public Value get();
}
```

At the opposite, a `PushMeasure` allows to obtain the value of a property in an asynchronous way, which means that the value is provided upon generation, the user having no control on when such a value will be provided to him. This is achieved by using an [observer design pattern](https://en.wikipedia.org/wiki/Observer_pattern), such that the user registers one or several `MeasureListener` instances to receive and process the value when it is produced:
```
public interface PushMeasure<Value> extends Measure<Value> {
	public void register(MeasureListener<Value> listener);
	public void unregister(MeasureListener<Value> listener);
}

public interface MeasureListener<Value> {
	public void measureGenerated(Value value);
}
```

Some people could wonder why these interfaces only require *reading* methods: the `PullMeasure` does not provide a `set(value)` method to assign its value, and the `PushMeasure` does not provide some kind of `push(value)` method neither. This is because these interfaces are designed from a user perspective, not an algorithm designer perspective, and the user can only read these values, not write them. One could say that it makes the thing harder for the designer, but actually the designer needs to know exactly which implementation to use, because he is the one who know how the values will be provided. So if he uses an existing implementation, he should of course know the specific methods of this implementation, which can include methods to set/push his values. Only the user does not need to know about the specific implementation used by the measure, so he is the one who will have to deal with generic `PullMeasure` and `PushMeasure`. Moreover, while it is natural to think about these set and push methods, it is actually not the only way to implement these measures. For instance, the algorithm designer could use a field to store the value of a property, and the update of this property (and the related `PullMeasure`) will be done through this variable rather than through the call of some methods. More detailed explanations are provided in the section [*How to create measures?*](#how-to-create-measures).

One could notice that both the measure interfaces extend `Measure`. This one is an empty interface which is used as a root interface to both `PullMeasure` and `PushMeasure`. By having it, we give the possibility for programers to manage measures in a generic way, without having to consider both types of measures separately nor to use `Object` to have them together. Thus, it is only here to simplify the use of measures for some highly generic cases in jMetal. No algorithm designer nor user should normally need it.

Additionally to the measures themselves, jMetal 5 also provides the notion of `MeasureManager`, which deals with measures management features:
```
public interface MeasureManager {
	public Collection<Object> getMeasureKeys();
	public <T> PullMeasure<T> getPullMeasure(Object key);
	public <T> PushMeasure<T> getPushMeasure(Object key);
}
```
You can notice that we provide a method for each type rather than a generic method returning a `Measure`. This is because, as mentionned before, the `Measure` interface is empty, thus has no practical value. Moreover, when the user want to exploit a measure, he should know which type of measure is implemented to know how to interact with it. Rather than providing a `Measure` and arbitrarily cast it, we prefered to provide methods which directly provide the right type of measure. Notice that a measure instance can implement both interfaces (or two instances can be made available for the same property), so both methods can return an instance (same or not) for the same key, giving to the user the choice of using one way or another. In the case where only one is provided (the other being `null`), it is possible to complete it, as described in the [section dedicated to conversions](#conversions-pullmeasure---pushmeasure). The key identifies the specific property to measure and is algorithm-dependent, justifying the presence of an additional `getMeasureKeys()` for the user to retrieve them.

Finally, in order for an algorithm to explicit that it provides measures, it should implement the `Measurable` interface, which simply requires to provide a `MeasureManager`:
```
public interface Measurable {
	public MeasureManager getMeasureManager();
}
```
So far, an `Algorithm` does not automatically implements `Measurable`, but it may change in future releases if we assess the relevance of the interface for a generic purpose.

One could wonder why we introduced the intermediary concept of `MeasureManager` rather than putting directly its methods into the `Measurable` interface. Indeed, by construction, the designer could simply decide to implement both the interfaces on the algorithm and implement `getMeasureManager()` by simply returning `this`, showing that we can artificially ignore the intermediary concept. Also, in the case where we actually reduce to the `Measurable` interface, the designer could add an intermediary objects which implements `Measurable` (so the methods of `MeasureManager`), and implement it also for the algorithm, but using his custom object in background. So technically, we see that introducing an intermediary notion of `MeasureManager` does not impose any constraint, justifying that we use the most simple design (no intermediary concept). Anyway, we made this design choice for the following reason: while the `MeasureManager` should focus on the measure management strategy, a `Measurable` should focus on which measures to provide. For instance, a `MeasureManager` could implement an advanced management strategy which, for measures implementing only one of the measure interfaces, would automatically instantiate a `PullMeasure`/`PushMeasure` in order to have all the features for each measure, with some smart inspection management for `PushMeasures` corresponding to `PullMeasures`. On the other hand, a `Measurable` instance, typically an algorithm, would focus on choosing which measures to provide and feeding them, delegating any measure management process to a dedicated `MeasureManager` implementation.

## Why using measures?

Usually, properties are accessed by getters, like `getPopulationSize()` or `getCurrentIteration()`. The advantage of this design is that it gives a simple way to access these properties. However, we quickly face the limitations of this design when we want to read properties which evolve in time, like the current iteration. Indeed, such a design imposes to read these properties on a regular basis, sometime on a frequent basis to see all the updates (also called *polling*, *spinning*, or *busy-waiting*). Such a design becomes particularly cumbersome when we want to access short-term values, like which individuals have been generated at a given iteration of a genetic algorithm. These individuals are usually forgotten at the next iteration (only the good ones are kept), thus imposing a frequent check. Accessing such properties at runtime would require whether to consume a lot of computation time to continuously inspect some `getGeneratedIndividuals()` method, or to consume a lot of space to store all the data generated and access it through some `getGeneratedIndividuals(int iteration)` method.

The design we choose for jMetal 5 is based on the notion of measure, which further split into two categories: `PullMeasure` and `PushMeasure`. The simplest one, the `PullMeasure`, is designed for the first kind of property, which can be easily accessed (pulled) from a getter. While one could simply use a getter, the `PullMeasure` provides a more generic access to the property, allowing to apply generic evaluations on the algorithm (like generic experiments, which are not yet available in jMetal 5.0). The other type of measure, the `PushMeasure`, is designed for the other kind of properties, which are not easily managed through getters and need to be provided (pushed) in real-time by the algorithm. By using such a measure, the values can be received and processed without risking to loose any update, and without the need to continuously inspect the property.

Another advantage of having both these measures is that it can be easily integrated to an algorithm without requiring significant additional resources: indeed, for cases where a value have to be stored into a variable for the algorithm to use it, like an iteration counter to stop after N iterations, such a value can be covered (or replaced) by a `PullMeasure`. At the opposite, when a value is generated but not stored during the running of the algorithm, a `PushMeasure` can be used to push the value to any potential listener and forget about it, letting the listeners decide whether or not this value should be stored or further processed. The additional resources consumed are only:
- the stored measures, which are often lightweight and less numerous than the solutions to store
- the calls to the listeners of the `PushMeasures`, which are negligible if no listener is registered, otherwise fully controlled by the user (not by *a priori* decisions from the algorithm designer)

## How to use measures?

Measures have been defined to be particularly easy to use. On one hand, a `PullMeasure` can be used basically like a getter, where instead of calling `getXxx()` we call `xxxMeasure.get()`. This results in using a `PullMeasure` directly when required by the user. On the other hand, because a `PushMeasure` only allows a user to register and unregister listeners (the notification generation is the responsibility of the algorithm), the user have no control on when the processing will occur: the process have to be put in the listener to exploit the data when it arrives, or the listener should store the value while letting another thread dealing with the processing. It is generally recommended to reduce the time spent in a listener to the minimum in order to let the source of the notification (the algorithm here) continues its job.

In other words, a process using `PullMeasures` should generally have this form, where the measures are used once the algorithm is running:
```
Algorithm<?> algorithm = new MyAlgorithm();

/* retrieval of the measures */
/* (only if the algorithm implements Measurable) */
MeasureManager measures = algorithm.getMeasureManager();
PullMeasure<Object> pullMeasure = measures.getPullMeasure(key);
...

/* preparation of the run */
...
/* run the algorithm in parallel */
Thread thread = new Thread(algorithm);
thread.start();

/* user process */
while (thread.isAlive()) {
	...
	/* use the value */
	Object value = pullMeasure.get();
	...
}
```

At the opposite, a process using `PushMeasures` should generally have this form, where the process is setup before to run the algorithm:
```
Algorithm<?> algorithm = new MyAlgorithm();

/* retrieval of the measures */
/* (only if the algorithm implements Measurable) */
MeasureManager measures = algorithm.getMeasureManager();
PushMeasure<Object> pushMeasure = measures.getPushMeasure(key);
pushMeasure.register(new MeasureListener<Object>() {
	
	@Override
	public void measureGenerated(Object value) {
		/* use the value */
		...
	}
});
...

/* preparation of the run */
...
/* run the algorithm in parallel */
Thread thread = new Thread(algorithm);
thread.start();

/* other processes */
while (thread.isAlive()) {
	...
}
```

In the case where only `PushMeasures` are used, one could also remove all the `Thread` management and simply call `algorithm.run()` and wait for it to finish. All the processes setup via `PushMeasures` will occur automatically.

## How to create measures?

### Create a `PullMeasure`

Usually, one implements an algorithm by storing some values in dedicated public fields, so a user can retrieve them on the fly. A really common example is a population of solutions, that we can find in many algorithms managing several solutions at the same time, like a genetic algorithm. Some others prefer to use getters, like `getPopulation()`, to provide a read-only access (while the field can be changed by the external user). These fields and getters are the best candidates for `PullMeasures`, because they can be wrapped in a straightforward manner. For our population example:
```
PullMeasure<Collection<Path>> populationMeasure = new PullMeasure<Collection<Path>>() {
	
	@Override
	public String getName() {
		return "population";
	}
	
	@Override
	public String getDescription() {
		return "The set of paths used so far.";
	}
	
	@Override
	public Collection<Path> get() {
		return getPopulation();
	}
};
```
The name and description are additional data to describe the measure itself, to know what it provides, and any measure should implement it, which makes the implementation of the interface quite heavy. However, this code can be reduced by using `SimplePullMeasure`, which takes the name and description in argument to focus on the value to retrieve:
```
PullMeasure<Collection<Path>> populationMeasure
= new SimplePullMeasure<Collection<Path>>("population",
                                          "The set of paths used so far.") {
	@Override
	public Collection<Path> get() {
		return getPopulation();
	}
};
```

If no getter is available, a field can also be used exactly the same way. These cases are the most basic uses of a `PullMeasure`. They are also the most common if you adapt an existing implementation to use the jMetal formalism. Indeed, using fields and getters is the simple way to provide an access to the internal data of an algorithm, which gives a lot of occasions to use `PullMeasures`. But these cases are not the only ones. Indeed, any computation can be defined in the `get()` method, which allows to add new measures even for inexistent fields and getters. For instance, assuming that the algorithm manages the time spent in some of its steps, it could store an internal `startTime` value which indicates when the algorithm have been started. From this variable, one could measure how long the algorithm has run:
```
PullMeasure<Long> runningTimeMeasure
= new SimplePullMeasure<Long>("running time",
                              "The time spent so far in running the algorithm.") {
	@Override
	public Long get() {
		return System.currentTimeMillis() - startTime;
	}
};
```
The advantage of putting the computation directly into the `get()` method is that the value is computed only when requested. Thus, it is the responsibility of the external user to decide when it is worth to compute it.

So far, we saw that a `PullMeasure` is basically used in the same way than a getter (we can also use a getter to make some computation). This is actually its principal purpose, but it does it in a standardised way: indeed, given that you have an algorithm which provides you some getters or equivalent, you can wrap all of them into `PullMeasures`, which gives you a unified way to access these values in a generic context (where you do not know which method to use nor how to use them, unless reflexion is used). Moreover, if you have an algorithm which provides a set of `PullMeasures`, you can extend them by creating new ones (while you cannot add getters nor fields to an instance):
```
PullMeasure<Integer> populationSizeMeasure
= new SimplePullMeasure<Integer>("population size",
                                 "The number of solutions used so far.") {
	@Override
	public Integer get() {
		// reuse a measure to compute another property
		return populationMeasure.get().size();
	}
};
```

With the ability to extend a set of measures, one can create the relevant measures for a specific experiments for instance (not yet implemented in jMetal 5.0). In other words, the algorithm designer can focus on providing a minimal set of measures and let the external user define new ones when required.

Finally, additional facilities are provided by jMetal to simplify the creation of `PullMeasures`. We already mentionned the `SimplePullMeasure` which focuses on defining the `get()` method, but in the case where the measure wraps a field, one could prefer to use directly the measure instead of the field itself by using a `BasicMeasure`, which directly stores the value by defining an additional `set(value)` method. More specific measures are also defined, like the `CountingMeasure` which allows to count occurrences, typically like a number of iterations or a number of solutions generated, or the `DurationMeasure` to evaluate the time spent in some activities. Several implementations of `PullMeasure` also implement `PushMeasure`, thus allowing a high flexibility on their use. In the case where one want to add `PullMeasures` to an existing algorithm, it is also possible to use the `MeasureFactory` to facilitate the instantiation of several `PullMeasures` at once:
- `createPullsFromFields(object)` instantiates a `PullMeasure` for each field of an object and returns a `Map` associating the name of each field to the corresponding measure,
- `createPullsFromGetters(object)` instantiates a `PullMeasure` for each getter in a similar way.

### Create a `PushMeasure`

A `PushMeasure` standardises the [observer design pattern](https://en.wikipedia.org/wiki/Observer_pattern) for algorithms. As an observer is supposed to be notified when the value it observes is updated, a `PushMeasure` notifies a listener (a broadly used term for observers in Java, especially in Swing) when a property of the algorithm changes. Noticeably, the interface `PushMeasure` is really reduced: it only requires the methods to add and remove listeners. Because of that, it is the responsibility of the measure implementer to decide how the listeners are notified. Several implementations are already provided in jMetal to simplify this work. In particular, probably most of the cases will find their way in using `SimplePushMeasure`, for instance if we want to notify when a new solution is generated:
```
SimplePushMeasure<MySolution> lastGeneratedSolution = new SimplePushMeasure<>(
		"last solution",
		"The last solution generated during the running of the algorithm.");
```
At the opposite of a passive `PullMeasure` (this is the user who decides when to call it), a `PushMeasure` is an active measure, in the sense that it is a particular event occuring during the run of the algorithm which triggers the notification process. For our example of last generated solution, we could have a basic hill-climbing method which starts from a random solution and then creates mutants to iteratively improve it. These random and mutant generations are the two relevant events in the algorithm for using our measure:
```
MySolution best = createRandomSolution();
lastGeneratedSolution.push(best);

while (running) {
	MySolution mutant = createMutantSolutionFrom(best);
	lastGeneratedSolution.push(mutant);
	
	// ...
	// remaining of the loop
	// ...
}
```

This example is illustrative in two ways: first, there can have *several* events to consider for a single measure, and second, the notification process should be done *as soon as* the event has occurred. This implies that a `PushMeasure` is generally deeply involved in the code of the algorithm itself, at the opposite of a `PullMeasure` which can wrap a field or a getter method, letting the algorithm itself untouched. Moreover, it also means that some extra computation time is consumed each time such a relevant event occurs. Because of that, a `PushMeasure` is well suited for notifying about a result *already computed* (because the algorithm need it) rather than to compute extra data for the sole purpose of measuring some properties. For an extra computation, it is wiser to exploit both a `PushMeasure`, to notify about the *already* computed stuff which serves as a basis for the extra computation (if any), with an additional `PullMeasure`, which will make the extra computation only if requested by the user.

Several implementations provided by jMetal already implement the `PushMeasure` interface. We already saw the `SimplePushMeasure`, which should be sufficient for many cases, but one can also notice the `CountingMeasure`, which allows to count the events (the value notified is an integer incremented at each notification). This implementation is for instance well suited for notifying the start/end of an iteration or how many solutions have been generated so far. It also implements the `PullMeasure` interface, allowing to retrieve the last value notified on demand.

### Conversions `PullMeasure` <-> `PushMeasure`

Some measures implement both `PullMeasure` and `PushMeasure`, but in the case where a single one is implemented, it is still possible to create another measure to complement it. This can be achieved by using the `MeasureFactory`, which provides conversions in both directions:
- `createPullFromPush(push, initialValue)` creates a `PullMeasure` from a `PushMeasure`. Every time the initial `PushMeasure` notifies its listeners, the `PullMeasure` is updated and stores the value for future calls of its `get()`. The `initialValue` provided to the method tells which value to use before the next notification occurs (typically `null` or the actual value if it is known).
- `createPushFromPull(pull, period)` creates a `PushMeasure` from a `PullMeasure`. Because there is no particular event produced by a `PullMeasure`, we artificially poll it (frequently check its value) at the given `period` to see when it changes. Identifying a change will result in generating a notification from the created `PushMeasure`. A short `period` offers a better reactivity but increases the computation cost, explaining why this method should not be used unless it is necessary. This is also why it is generally preferable, when it is possible to choose, to setup a `PushMeasure` rather than a `PullMeasure`: the conversion costs way less in that direction.

### Add measures to an algorithm

In order for an algorithm to provide measures, it should implement the `Measurable` interface, which asks to provide a `MeasureManager`. This manager is the one storing and giving access to all the measures of the algorithm. While one can implement his own manager, jMetal already provide the `SimpleMeasureManager` implementation which provides the following methods:
```
public class SimpleMeasureManager implements MeasureManager {

	// Methods to configure the PullMeasures
	public void setPullMeasure(Object key, PullMeasure<?> measure) {...}
	public <T> PullMeasure<T> getPullMeasure(Object key) {...}
	public void removePullMeasure(Object key) {...}
	
	// Methods to configure the PushMeasures
	public void setPushMeasure(Object key, PushMeasure<?> measure) {...}
	public <T> PushMeasure<T> getPushMeasure(Object key) {...}
	public void removePushMeasure(Object key) {...}

	// Methods to configure any measure (auto-recognition of the type)
	public void setMeasure(Object key, Measure<?> measure) {...}
	public void removeMeasure(Object key) {...}
	public void setAllMeasures(Map<? extends Object, ? extends Measure<?>> measures) {...}
	public void removeAllMeasures(Iterable<? extends Object> keys) {...}
	
	// Provide the keys of the configured measures
	public Collection<Object> getMeasureKeys() {...}
}
```

While there is the basic, type-specific methods, there is also generic methods which automatically recognize the type of the measure provided, and apply the corresponding type-specific methods. Measures which implement both `PullMeasure` and `PushMeasure` are also recognized and added both as a `PullMeasure` and a `PushMeasure`, so calling `getPullMeasure(key)` and `getPushMeasure(key)` with the same `key` will return the same measure. The generic methods also provide a massive configuration feature by managing several keys and measures at once.

It is worth noting that, if an instance of a *non-jMetal* algorithm is provided, one can easily try to retrieve some measures from it by using `MeasureFactory.createPullsFromFields(object)` and `MeasureFactory.createPullsFromGetters(object)`. The maps returned by these two methods can then be provided to `SimpleMeasureManager.setAllMeasures(measures)` to have a fully featured, ready to use `MeasureManager`, without knowing anything about the actual algorithm. Given that we know how to run it, it is then possible to run it in a dedicated thread, as described in the section [*How to use measures?*](#how-to-use-measures), and to exploit the available measures to obtain some information about the algorithm. However, as underlined in the section [*Conversions `PullMeasure` <-> `PushMeasure`*](#conversions-pullmeasure---pushmeasure), it is costly to make `PushMeasures` from `PullMeasures`, while the reverse is quite cheap. Thus, although it can be tempting to simply implement an algorithm independently of jMetal and use this procedure to obtain a set of `PullMeasures`, someone designing an algorithm with the possibility to use the formalism of jMetal should focus on `PushMeasures` (or a combination of both) to retrieve more information in a more optimized way.