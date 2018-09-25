## Algorithm templates

Most of metaheuristic families are characterized by a common behaviour which is shared by all the algorithms belonging to the family. This behaviour can be expressed as a template that can be instatiated to implement a particular algorithm. From a software engineering point of view, an algorithm whose behavior falls in a basic template would only require to implement some specific methods for the new technique; the common behavior would not be needed to be programmed, therefore resulting in less code replication. This inversion of control if a characteristic of [software frameworks](https://en.wikipedia.org/wiki/Software_framework), as is the case of jMetal.

### The Evolutionary Algorithm Template
Many papers about evolutionary algorithms (EAs) include a pseudo-code to describe them similar to this one:  
```
P(0) ← GenerateInitialSolutions() 
t ← 0
Evaluate(P(0))
while not StoppingCriterion() do
  P'(t) ← selection(P(t))
  P''(t) ← Variation(P'(t)) 
  Evaluate(P''(t))
  P (t + 1) ← Update(P (t), P''(t)) 
  t←t+1
end while
```

To mimic this pseudo-code, jMetal 5 incorporates a template in the form of an abstract class named [`AbstractEvolutionaryAlgorithm`](https://github.com/jMetal/jMetal/blob/jmetal-5.0/jmetal-core/src/main/java/org/uma/jmetal/algorithm/impl/AbstractEvolutionaryAlgorithm.java), which contains the following code:
```java
package org.uma.jmetal.algorithm.impl;

/**
 * Created by Antonio J. Nebro on 26/10/14.
 * @param <S> Solution
 * @param <R> Result
 */
public abstract class AbstractEvolutionaryAlgorithm<S extends Solution<?>, R>  implements Algorithm<R>{
  private List<S> population;
  public List<S> getPopulation() {
    return population;
  }
  public void setPopulation(List<S> population) {
    this.population = population;
  }

  protected abstract void initProgress();
  protected abstract void updateProgress();
  protected abstract boolean isStoppingConditionReached();
  protected abstract List<S> createInitialPopulation();
  protected abstract List<S> evaluatePopulation(List<S> population);
  protected abstract List<S> selection(List<S> population);
  protected abstract List<S> reproduction(List<S> population);
  protected abstract List<S> replacement(List<S> population, List<S> offspringPopulation);
  @Override public abstract R getResult();

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
}  
```
The generics in the class declaration indicate that an algorithm works with subclasses of the `Solution` interface (e.g., `DoubleSolution`, `BinarySolution`, and so on) and returns a result (typically, a single solution in the case of single-objective metaheuristics and a list of solutions in the case of multi-objective techniques). We can observe as the population is implemented a list of solutions.

To develop an EA, all the abstract the methods used in the `run()` method must be implemented. We describe those methods next:
* `createInitialPopulation()`: This method fills the population with a set of tentative solutions. The typical strategy consists in generating randomly initialized solutions, but any other approach can be applied.
* `evaluatePopulation(population)`: All the solutions in the `population` argument are evaluated and a population, which can be the same one passed as a parameter or a new one, is returned as a result.
* `initProgress()`: The progress of an EA is usually measured by counting iterations or function evaluations. This method initializes the progess counter.
* `isStoppingConditionReached()`: the stopping condition establishes when the algorithm finishes its execution.
* `selection(population)`: the selection method chooses a number of solutions from the population to become the mating pool.
* `reproduction(matingPopulation)`: the solutions in the mating pool are manipulated somehow, by modifying them or by using them to create new ones, yielding to new solutions that constitute the offspring population.
* `replacement(population, offspringPopulation)`: the population for the next generation is built from individuals of the current and the offspring populations.
* `updateProgress()`: the counter of the progress of the algorithm (evaluations, iterations, or whatever) is updated.

#### Genetic algorithms 
If we are interested in implementing a genetic algorithm, a subfamily of EAs characterized by applying a selection operator and by using a crossover and a mutation operator for the reproduction step, a subclass of `AbstractEvolutionaryAlgorithm` called [AbstractGeneticAlgorithm](https://github.com/jMetal/jMetal/blob/jmetal-5.0/jmetal-core/src/main/java/org/uma/jmetal/algorithm/impl/AbstractGeneticAlgorithm.java) is provided:
```java
package org.uma.jmetal.algorithm.impl;

/**
 * Created by ajnebro on 26/10/14.
 */
public abstract class AbstractGeneticAlgorithm<S extends Solution<?>, Result> extends AbstractEvolutionaryAlgorithm<S, Result> {
  protected SelectionOperator<List<S>, S> selectionOperator ;
  protected CrossoverOperator<S> crossoverOperator ;
  protected MutationOperator<S> mutationOperator ;
}
```
Popular metaheuristics such as [NSGA-II](https://github.com/jMetal/jMetal/blob/jmetal-5.0/jmetal-algorithm/src/main/java/org/uma/jmetal/algorithm/multiobjective/nsgaii/NSGAII.java), [SPEA2](https://github.com/jMetal/jMetal/blob/jmetal-5.0/jmetal-algorithm/src/main/java/org/uma/jmetal/algorithm/multiobjective/spea2/SPEA2.java), [PESA2](https://github.com/jMetal/jMetal/blob/jmetal-5.0/jmetal-algorithm/src/main/java/org/uma/jmetal/algorithm/multiobjective/pesa2/PESA2.java), [MOCell](https://github.com/jMetal/jMetal/blob/jmetal-5.0/jmetal-algorithm/src/main/java/org/uma/jmetal/algorithm/multiobjective/nsgaii/NSGAII.java) or [SMS-EMOA](https://github.com/jMetal/jMetal/blob/jmetal-5.0/jmetal-algorithm/src/main/java/org/uma/jmetal/algorithm/multiobjective/smsemoa/SMSEMOA.java) are based on this template.

#### Evolution strategies
Another subfamily of EAs are evolution strategies, which are based on applying only mutation in the reproduction step. The corresponding abstract class for EAs is [`AbstractEvolutionStragegy`](https://github.com/jMetal/jMetal/blob/jmetal-5.0/jmetal-core/src/main/java/org/uma/jmetal/algorithm/impl/AbstractEvolutionStrategy.java):

```java
package org.uma.jmetal.algorithm.impl;

/**
 * Created by ajnebro on 26/10/14.
 */
public abstract class AbstractEvolutionStrategy<S extends Solution<?>, Result> extends AbstractEvolutionaryAlgorithm<S, Result> {
  protected MutationOperator<S> mutationOperator ;
}
```
The [PAES](https://github.com/jMetal/jMetal/blob/jmetal-5.0/jmetal-algorithm/src/main/java/org/uma/jmetal/algorithm/multiobjective/paes/PAES.java) algorithm is based on this template

TO BE COMPLETED
