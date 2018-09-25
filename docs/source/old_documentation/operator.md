## The `Operator` interface
Metaheuristic techniques are based on modifying or generating new solutions from existing ones by
means of the application of different operators. For example, EAs make use of crossover, mutation, and
selection operators for modifying solutions. In jMetal, any operation altering or generating solutions (or
sets of them) implements or extends the `Operator` interface:

``` java
package org.uma.jmetal.operator;

/**
 * Interface representing an operator
 *
 * @author Antonio J. Nebro <antonio@lcc.uma.es>
 * @version 0.1
 * @param <Source> Source Class of the object to be operated with
 * @param <Result> Result Class of the result obtained after applying the operator
 */
public interface Operator<Source, Result> {
  /**
   * @param source The data to process
   */
  public Result execute(Source source) ;
}

```
The generics in this interface are intended to indicate that an operator is applied to a `Source` object and returns as a result  `Result` object. 


The framework already incorporates a number of operators, which can be classiffed into four different
classes:
* Crossover. Represents the recombination or crossover operators used in EAs. Some of the included
operators are the simulated binary (SBX) crossover and the single-point crossover for real and
binary encodings, respectively.
* Mutation. Represents the mutation operator used in EAs. Examples of included operators are
polynomial mutation (real encoding) and bit-flip mutation (binary encoding).
* Selection. This kind of operator is used for performing the selection procedures in many metaheuristics. An
example of selection operator is the binary tournament.
* LocalSearch. This class is intended for representing local search procedures. It contains a  method for consulting how many evaluations have been performed after been applied.

We review the interfaces and implementations of these operators next.

### Crossover operators
The `CrossoverOperator` interface represents any crossover in jMetal 5:
```java
package org.uma.jmetal.operator;

/**
 * Interface representing crossover operators. They will receive a list of solutions and return
 * another list of solutions
 *
 * @author Antonio J. Nebro <antonio@lcc.uma.es>
 *
 * @param <S> The class of the solutions
 */
public interface CrossoverOperator<S extends Solution<?>> extends Operator<List<S>,List<S>> {
}
```
This interface simply states that a crossover has as a source a list of `Solution` objects and return as a result another list of solutions. Let us examine two implementations of this interface, one for double solutons and another one for binary solutions. 

The simulated binary crossover (SBX) is the default crossover operator in many multiobjective evolutionary algorithms (e.g., NSGA-II, SPEA2, SMS-EMOA, MOCell, etc). A scheme of the `SBXCrossover` class is shown next:
```java
package org.uma.jmetal.operator.impl.crossover;

/**
 * This class allows to apply a SBX crossover operator using two parent solutions (Double encoding).
 * A {@link RepairDoubleSolution} object is used to decide the strategy to apply when a value is out
 * of range.
 *
 * The implementation is based on the NSGA-II code available in
 * <a href="http://www.iitk.ac.in/kangal/codes.shtml">http://www.iitk.ac.in/kangal/codes.shtml</a>
 *
 * @author Antonio J. Nebro <antonio@lcc.uma.es>
 * @author Juan J. Durillo
 */
public class SBXCrossover implements CrossoverOperator<DoubleSolution> {
  /** EPS defines the minimum difference allowed between real values */
  private static final double EPS = 1.0e-14;

  private double distributionIndex ;
  private double crossoverProbability  ;
  private RepairDoubleSolution solutionRepair ;

  private JMetalRandom randomGenerator ;

  /** Constructor */
  public SBXCrossover(double crossoverProbability, double distributionIndex) {
    this (crossoverProbability, distributionIndex, new RepairDoubleSolutionAtBounds()) ;
  }

  /** Constructor */
  public SBXCrossover(double crossoverProbability, double distributionIndex, RepairDoubleSolution solutionRepair) {
    if (crossoverProbability < 0) {
      throw new JMetalException("Crossover probability is negative: " + crossoverProbability) ;
    } else if (distributionIndex < 0) {
      throw new JMetalException("Distribution index is negative: " + distributionIndex);
    }

    this.crossoverProbability = crossoverProbability ;
    this.distributionIndex = distributionIndex ;
    this.solutionRepair = solutionRepair ;

    randomGenerator = JMetalRandom.getInstance() ;
  }

  /** Execute() method */
  @Override
  public List<DoubleSolution> execute(List<DoubleSolution> solutions) {
    if (null == solutions) {
      throw new JMetalException("Null parameter") ;
    } else if (solutions.size() != 2) {
      throw new JMetalException("There must be two parents instead of " + solutions.size()) ;
    }

    return doCrossover(crossoverProbability, solutions.get(0), solutions.get(1)) ;
  }
  
  ...
```

TO BE COMPLETED
