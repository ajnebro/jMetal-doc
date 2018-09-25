## The `Algorithm` interface

A metaheuristic or algorithm in jMetal 5 is an entity that implements the `Algorithm` interface:
```java
package org.uma.jmetal.algorithm;

/**
 * Interface representing an algorithm
 * @author Antonio J. Nebro
 * @version 0.1
 * @param <Result> Result
 */
public interface Algorithm<Result> extends Runnable {
  void run() ;
  Result getResult() ;
}

```
This interface is very generic: it specifies that an algorithm must have a `run()` method and return a result by the `getResult()` method. As it extends `Runnable`, any algorithm can be executed in a thread.
 
The symplicity of `Algorithm` offers plenty of freedom to implement a metaheuristic according to your favorite preferences. However, as jMetal 5 is a framework it includes a set of resources and strategies to help in the implementation of algorithms with the idea of promoting good design, code reusing, and flexibility. The key components are the use of the [builder pattern](https://en.wikipedia.org/wiki/Builder_pattern) and [algorithm templates](https://github.com/jMetal/jMetalDocumentation/blob/master/algorithmTemplates.md). In the next section we give a detailed description of how the well-known NSGA-II algorithm is implemented, configured, and extended.

### Case study: NSGA-II

NSGA-II is a genetic algorithm (GA), i.e. it belongs to the evolutionary algorithms (EAs) family. The implementation of NSGA-II provided in jMetal 5.0 follows the evolutionary algorithm template described in the [algorithm templates](https://github.com/jMetal/jMetalDocumentation/blob/master/algorithmTemplates.md) section of the documentation. This means that it must define the methods of the [`AbstractEvolutionaryAlgorithm`](https://github.com/jMetal/jMetal/blob/jmetal-5.0/jmetal-core/src/main/java/org/uma/jmetal/algorithm/impl/AbstractEvolutionaryAlgorithm.java) class. According to this template, the flow control of the algorithm is defined in the `run()` method:
```java
@Override public void run() {
    List<S> offspringPopulation;
    List<S> matingPopulation;

    population = createInitialPopulation();
    population = evaluatePopulation(population);
    initProgress();
    while (!isStoppingConditionReached()) {
      matingPopulation = selection(population);
      offspringPopulation = reproduction(matingPopulation);
      offspringPopulation = evaluatePopulation(offspringPopulation);
      population = replacement(population, offspringPopulation);
      updateProgress();
    }
  }
  ```

We describe next how these methods are implemented in the [NSGAII](https://github.com/jMetal/jMetal/blob/jmetal-5.0/jmetal-algorithm/src/main/java/org/uma/jmetal/algorithm/multiobjective/nsgaii/NSGAII.java) class.

The class declaration is as follows:
```java
public class NSGAII<S extends Solution<?>> extends AbstractGeneticAlgorithm<S, List<S>> {
   ...
}
```
which indicates that it extends the [`AbstractGeneticAlgorithm`](https://github.com/jMetal/jMetal/blob/jmetal-5.0/jmetal-core/src/main/java/org/uma/jmetal/algorithm/impl/AbstractGeneticAlgorithm.java). The generic `S` allows to specify the encoding of the solutions that will manipulate the algorithm, and it will determine the kind of problems that can be solved as well as the operators that can be used. This is exemplified in the class constructor:

```java
 public NSGAII(Problem<S> problem, int maxIterations, int populationSize,
      CrossoverOperator<S> crossoverOperator, MutationOperator<S> mutationOperator,
      SelectionOperator<List<S>, S> selectionOperator, SolutionListEvaluator<S> evaluator) {
    super() ;
    this.problem = problem;
    this.maxIterations = maxIterations;
    this.populationSize = populationSize;

    this.crossoverOperator = crossoverOperator;
    this.mutationOperator = mutationOperator;
    this.selectionOperator = selectionOperator;

    this.evaluator = evaluator;
  }
```
The constructor parameter contains:

* The problem to solve.
* The main algorithm parameters: the population size and the maximum number of iterations.
* The genetic operators: crossover, mutation, and selection.
* An [evaluator](https://github.com/jMetal/jMetalDocumentation/blob/master/evaluators.md) object to evaluate the solutions in the population.

We can observe that all the parameters depend on `S`. This way, if `S` is instantiated e.g. to [`DoubleSolution`](https://github.com/jMetal/jMetal/blob/jmetal-5.0/jmetal-core/src/main/java/org/uma/jmetal/solution/DoubleSolution.java), then the problems to be solved must extend `Problem<DoubleSolution>` and all the operators must manipulate `DoubleSolution` objects. The interesting point of this approch is the compiler can ensure that there are no errors related with the application of wrong operators to a given solution.

The default `createInitialPopulation()` method adds a number of `populationSize` new solutions to a list:

```java
  @Override protected List<S> createInitialPopulation() {
    List<S> population = new ArrayList<>(populationSize);
    for (int i = 0; i < populationSize; i++) {
      S newIndividual = problem.createSolution();
      population.add(newIndividual);
    }
    return population;
  }
```

The evalution of lists of solutions are delegated to `Evaluator` objects, so the `evaluatePopulation()` method is very simple:

```java
  @Override protected List<S> evaluatePopulation(List<S> population) {
    population = evaluator.evaluate(population, problem);

    return population;
  }
```

The NSGA-II implementation assumes that the stopping condition will be defined around a maximum number of iterations:

```java
  @Override protected boolean isStoppingConditionReached() {
    return iterations >= maxIterations;
  }
```

so the `initProgress()` method initalizes the iteration counter (the initial value is 1 because it is assumed that the initial populatio has been already evaluated):

```java
  @Override protected void initProgress() {
    iterations = 1;
  }
```

and the `updateProgress()` method merely increments the counter:

```java
  @Override protected void updateProgress() {
    iterations++;
  }

```

Accordig to the EA template, the `Selection()` method must create a mating pool from the population, so it is implemented this way:

```java
  @Override protected List<S> selection(List<S> population) {
    List<S> matingPopulation = new ArrayList<>(population.size());
    for (int i = 0; i < populationSize; i++) {
      S solution = selectionOperator.execute(population);
      matingPopulation.add(solution);
    }

    return matingPopulation;
  }
```

and the `reproduction()` method applies the crossover and mutation operators to the mating population, leading to new individuals that are added to an offspring population:

```java
  @Override protected List<S> reproduction(List<S> population) {
    List<S> offspringPopulation = new ArrayList<>(populationSize);
    for (int i = 0; i < populationSize; i += 2) {
      List<S> parents = new ArrayList<>(2);
      parents.add(population.get(i));
      parents.add(population.get(i + 1));

      List<S> offspring = crossoverOperator.execute(parents);

      mutationOperator.execute(offspring.get(0));
      mutationOperator.execute(offspring.get(1));

      offspringPopulation.add(offspring.get(0));
      offspringPopulation.add(offspring.get(1));
    }
    return offspringPopulation;
  }
```
Finally, the `replacement()` method joins the current and offspring populations to produce the population of the next generation by applying the ranking and crowding distance selection:

```java
  @Override protected List<S> replacement(List<S> population, List<S> offspringPopulation) {
    List<S> jointPopulation = new ArrayList<>();
    jointPopulation.addAll(population);
    jointPopulation.addAll(offspringPopulation);

    Ranking<S> ranking = computeRanking(jointPopulation);

    return crowdingDistanceSelection(ranking);
  }
```

### Case study: Steady-state NSGA-II
An advantage of using the EA template to implement NSGA-II is that it allows to simplify the implementation of variants of the algorithm. To give an example, we describe here the [SteadyStateNSGAII](https://github.com/jMetal/jMetal/blob/jmetal-5.0/jmetal-algorithm/src/main/java/org/uma/jmetal/algorithm/multiobjective/nsgaii/SteadyStateNSGAII.java) class, which implements a steady-state version of NSGA-II. This version is basically NSGA-II but with an auxiliar population of size 1, so the `SteadyStateNSGAII` is an extension of class [`NSGAII`](https://github.com/jMetal/jMetal/blob/jmetal-5.0/jmetal-algorithm/src/main/java/org/uma/jmetal/algorithm/multiobjective/nsgaii/NSGAII.java):

```java
public class SteadyStateNSGAII<S extends Solution<?>> extends NSGAII<S> {
}
```

and the class constructor is similar to the one of NSGA-II:

``` java
  public SteadyStateNSGAII(Problem<S> problem, int maxIterations, int populationSize,
      CrossoverOperator<S> crossoverOperator, MutationOperator<S> mutationOperator,
      SelectionOperator<List<S>, S> selectionOperator, SolutionListEvaluator<S> evaluator) {
    super(problem, maxIterations, populationSize, crossoverOperator, mutationOperator,
        selectionOperator, evaluator);
  }
```

The only differences between the two algorithm variants are in the `selection()` (the mating pool is composed of two parents) and `reproduction()`(only a child is generated) methods:

```java
  @Override protected List<S> selection(List<S> population) {
    List<S> matingPopulation = new ArrayList<>(2);

    matingPopulation.add(selectionOperator.execute(population));
    matingPopulation.add(selectionOperator.execute(population));

    return matingPopulation;
  }

  @Override protected List<S> reproduction(List<S> population) {
    List<S> offspringPopulation = new ArrayList<>(1);

    List<S> parents = new ArrayList<>(2);
    parents.add(population.get(0));
    parents.add(population.get(1));

    List<S> offspring = crossoverOperator.execute(parents);

    mutationOperator.execute(offspring.get(0));

    offspringPopulation.add(offspring.get(0));
    return offspringPopulation;
  }
```

This way, most of the code of the `NSGAII` class is reused and only two methods have had to be redefined.

### Using the builder pattern to configure NSGA-II
To configure the algorithms in jMetal 5 we have adopted the approach of using the builder pattern, which is represented by the [`AlgorithmBuilder`](https://github.com/jMetal/jMetal/blob/jmetal-5.0/jmetal-core/src/main/java/org/uma/jmetal/util/AlgorithmBuilder.java) interface:

```java
/**
 * Interface representing algorithm builders
 *
 * @author Antonio J. Nebro <antonio@lcc.uma.es>
 */
public interface AlgorithmBuilder<A extends Algorithm<?>> {
  public A build() ;
}
```




TO BE COMPLETED
