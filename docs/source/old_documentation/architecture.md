<!--<div id='id-architecture'/>-->
## Architecture

The architecture of jMetal 5 relies on four interfaces: 

![jMetal architecture](https://github.com/jMetal/jMetalDocumentation/blob/master/figures/jMetal5CoreClassDiagram.png)

This diagram captures the typical functionality provided by jMetal: an `Algorithm` solves a `Problem` by manipulating a set of potential `Solution` objects through the use of several `Operators`. The `Solution` interface represents the individuals in evolutionary algorithms and the particles in the case of particle swarm optmization algorithms. A `Problem` can create new solutions and evaluate them. 
Compared to previous versions of jMetal, there is not a class for the concept of population or swarm. In jMetal 5 a population is merely a list of solutions (`List<Solution>` in Java).


### Generics
We can observe the use of parametrized types to model the use of Java generics, which are now widely applied.
 
The use of generics in the architecture allows to align all the components in metaheuristic so that the Java compiler can check that everything fit. For example, this code represents all the elements to configure a the well-known NSGA-II algorithm to solve a continuous problem:

```java
    Problem<DoubleSolution> problem;
    Algorithm<List<DoubleSolution>> algorithm;
    CrossoverOperator<DoubleSolution> crossover;
    MutationOperator<DoubleSolution> mutation;
    SelectionOperator<List<DoubleSolution>, DoubleSolution> selection;

    ...

    algorithm = new NSGAIIBuilder<DoubleSolution>(problem, crossover, mutation)
        .setSelectionOperator(selection)
        .setMaxEvaluations(25000)
        .setPopulationSize(100)
        .build() ;
```

### Hierarchy of `Algorithm` related classes

The `Algorithm` class is very simple and it contain only two methods,  `run()` y `getResult()`, as can be observed in the following code snippet:

```java
package org.uma.jmetal.algorithm;

/**
 * Interface representing an algorithm
 * @author Antonio J. Nebro
 * @version 0.1
 * @param <Result> Result
 */
public interface Algorithm<Result> extends Runnable, Serializable, DescribedEntity {
  void run() ;
  Result getResult() ;
}

```

jMetal 5 includes a hierarchy of classes that inherits from `Algorithm`, as depicted in the following diagram: 

![jMetal architecture](https://github.com/jMetal/jMetalDocumentation/blob/master/figures/algorithmHierarchy.png)

On the one hand, we found a level of abstract classes (e.g., `AbstractEvolutionaryAlgorithm` or `AbstractParticleSwarmOptimization`) which constitute templates than can be used to facilitate the implementation of algorithms by reusing an extending the already provided code. On the other hand, we can see two examples of algorithms, MOEA/D and NSGAII45, which do not follow none of the provided templates. This way you are free to implement a new algorithm on your own or by extending some of the existing classes.

We can observe that, in the case of NSGA-II, it inherits from `AbstractGeneticAlgorithm`, which is a subclass of `AbstractEvolutionaryAlgorithm`. The diagram shows that a steady-state variant of NSGA-II can be defined by extending the `NSGAII` class.