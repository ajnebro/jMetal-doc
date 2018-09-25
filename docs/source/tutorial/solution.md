## The `Solution` interface

One of the first decisions that have to be taken when using metaheuristics is to define how to encode
or represent the tentative solutions of the problem to solve. Representation strongly depends on the
problem and determines the operations (e.g., recombination with other solutions, local search procedures,
etc.) that can be applied. Thus, selecting a specific representation has a great impact on the behavior
of metaheuristics and, hence, in the quality of the obtained results.

The following figure depicts the basic components that are used for representing solutions in jMetal 5:
![The Solution Interface](https://github.com/jMetal/jMetalDocumentation/blob/master/figures/jMetal5SolutionClassDiagram.png)
where three representations are included: binary, real, and integer. By using this approach, many implementations can be provided for the same encoding, adding an extra degree of flexibility. The use of generics also allows that an attempt to incorrectly assign the value of a variable results in a compilation error, e.g., trying to assign to an int variable the variable value of a `DoubleSolution`.

The code of the `Solution` interface is shown next:
```java
package org.uma.jmetal.solution;

public interface Solution<T> extends Serializable {
  public void setObjective(int index, double value) ;
  public double getObjective(int index) ;

  public T getVariableValue(int index) ;
  public void setVariableValue(int index, T value) ;
  public String getVariableValueString(int index) ;

  public int getNumberOfVariables() ;
  public int getNumberOfObjectives() ;

  public Solution<T> copy() ;

  public void setAttribute(Object id, Object value) ;
  public Object getAttribute(Object id) ;
}
```

The interface has methods for accessing both the variables and the objectives of a solution, a copy method, and to methods for accessing solution atributes. 

### Defining encodings
Defining a particular encoding implies implementing or extending the `Solution` interface. This way, the interfaces for solutions having a list of double and integer variables are defined as follows:
```java
package org.uma.jmetal.solution;

public interface DoubleSolution extends Solution<Double> {
  public Double getLowerBound(int index) ;
  public Double getUpperBound(int index) ;
}
```
```java 
package org.uma.jmetal.solution;

public interface IntegerSolution extends Solution<Integer> {
  public Integer getLowerBound(int index) ;
  public Integer getUpperBound(int index) ;
}
``` 
These interfaces provide for getting the lower and upper bounds of the double and integer variables. The way of setting those values are left to the implementation classes.

In the case of a binary solution, the interface is: 
```java
import org.uma.jmetal.util.binarySet.BinarySet;

public interface BinarySolution extends Solution<BinarySet> {
  public int getNumberOfBits(int index) ;
  public int getTotalNumberOfBits() ;
}
```

assuming that we intend to represent a list of binary variables.

The adopted approach allows to define encodings having mixed variables. For example, this interface defines solutions composed of lists of double and integer values:
```java
package org.uma.jmetal.solution;

public interface IntegerDoubleSolution extends Solution<Number> {
  public Number getLowerBound(int index) ;
  public Number getUpperBound(int index) ;
  public int getNumberOfIntegerVariables() ;
  public int getNumberOfDoubleVariables() ;
}
```
### Implementing solutions
Once we have defined a set of interfaces for the different solutions, we provide default implementions to all of them. Our approach is to take as starting point an abstract class named `AbstractGenericSolution`:
```java
package org.uma.jmetal.solution.impl;

public abstract class AbstractGenericSolution<T, P extends Problem<?>> implements Solution<T> {
  private double[] objectives;
  private List<T> variables;
  protected P problem ;
  protected double overallConstraintViolationDegree ;
  protected int numberOfViolatedConstraints ;
  protected Map<Object, Object> attributes ;
  protected final JMetalRandom randomGenerator ;
```
which contains an implementation to all the methods in `Solution`. This class is extended by all the solution implementations in jMetal 5: `DefaultBinarySolution`, `DefaultIntegerSolution`, `DefaultDoubleSolution`, `DefaultIntegerDoubleSolution`, `DefaultIntegerPermutationSolution`, and `DefaultDoubleBinarySolution`. 

### Where are the populations?

In jMetal 5 there is not any class to represent the concept of population. Instead, a Java `List` of `Solution` objects is used.

Some examples:
``` java
/* A population of double solutions */
List<DoubleSolution> doublePopulation ;

/* The same population using the generic interface */
List<Solution<Double>> doublePopulation ;

/* A population of binary solutions */
List<BinarySolucion> binaryPopulation ;
```

An utility class called [`SolutionListUtils`](https://github.com/jMetal/jMetal/blob/master/jmetal-core/src/main/java/org/uma/jmetal/util/SolutionListUtils.java) offers a set of operations over solution lists, such as finding the best/worst solution, selecting solutions randomly, etc.

### Solution attributes
The idea of incorporating attributes is to allow to add specific fields to solutions that are needed by some algorithms. For example, NSGA-II requires to rank the solutions and assign them the value of the crowding distance, while SPEA2 assigns a raw fitness to the solutions.

The attributes manipulated directly, but we include also this utility interface:
```java
package org.uma.jmetal.util.solutionattribute;
/**
 * Attributes allows to extend the {@link Solution} classes to incorporate data required by
 * operators or algorithms manipulating them.
 *
 * @author Antonio J. Nebro <antonio@lcc.uma.es>
 */
public interface SolutionAttribute <S extends Solution<?>, V> {
  public void setAttribute(S solution, V value) ;
  public V getAttribute(S solution) ;
  public Object getAttributeID() ;
}
```

and a default implementation:
```java
package org.uma.jmetal.util.solutionattribute.impl;

public class GenericSolutionAttribute <S extends Solution<?>, V> implements SolutionAttribute<S, V>{

  @SuppressWarnings("unchecked")
  @Override
  public V getAttribute(S solution) {
    return (V)solution.getAttribute(getAttributeID());
  }

  @Override
  public void setAttribute(S solution, V value) {
     solution.setAttribute(getAttributeID(), value);
  }

  @Override
  public Object getAttributeID() {
    return this.getClass() ;
  }
}
```
Note that in the current implementation the `getAttributedID()` returns a class identifier. This means that we cannot have two different attributes of the same class. 

### Example of attribute: constraints
Optimization problems can have side constraints, and this implies that evaluating a solution requires to compute the objective functions and also the constraints to apply some kind of constraint handling mechanism. In jMetal 5 solution attributes are used to incorporate constraint information into the solutions.

The default constraint handling mechanism in jMetal is the overall constraing violation scheme defined in NSGA-II, so the following class is provided:

```java
package org.uma.jmetal.util.solutionattribute.impl;
public class OverallConstraintViolation<S extends Solution<?>> extends GenericSolutionAttribute<S, Double> {
}
```
It is an empty class extending `GenericSolutionAttribute` specifying a double value for the attribute. Typically, the constraints are evaluted in the class defining the problem as is shown in this example:
```java
package org.uma.jmetal.problem.multiobjective;

/** Class representing problem Binh2 */
public class Binh2 extends AbstractDoubleProblem implements ConstrainedProblem<DoubleSolution> {
  public OverallConstraintViolation<DoubleSolution> overallConstraintViolationDegree ;
  public NumberOfViolatedConstraints<DoubleSolution> numberOfViolatedConstraints ;
  /**
   * Constructor
   * Creates a default instance of the Binh2 problem
   */
  public Binh2() {
    ...
    overallConstraintViolationDegree = new OverallConstraintViolation<DoubleSolution>() ;
    numberOfViolatedConstraints = new NumberOfViolatedConstraints<DoubleSolution>() ;
  }

  /** Evaluate() method */
  @Override
  public void evaluate(DoubleSolution solution) {
     ...
  }

  /** EvaluateConstraints() method */
  @Override
  public void evaluateConstraints(DoubleSolution solution)  {
    double[] constraint = new double[this.getNumberOfConstraints()];

    double x0 = solution.getVariableValue(0) ;
    double x1 = solution.getVariableValue(1) ;

    constraint[0] = -1.0 * (x0 - 5) * (x0 - 5) - x1 * x1 + 25.0;
    constraint[1] = (x0 - 8) * (x0 - 8) + (x1 + 3) * (x1 + 3) - 7.7;

    double overallConstraintViolation = 0.0;
    int violatedConstraints = 0;
    for (int i = 0; i < this.getNumberOfConstraints(); i++) {
      if (constraint[i] < 0.0) {
        overallConstraintViolation += constraint[i];
        violatedConstraints++;
      }
    }

    overallConstraintViolationDegree.setAttribute(solution, overallConstraintViolation);
    numberOfViolatedConstraints.setAttribute(solution, violatedConstraints);
  }
```
This code includes also another attribute, called `NumberOfViolatedConstraints` that is used to set the number of violated constraints of a given solution.

### Example of attribute: ranking

The use of solution attributes can be encapsulated. As an example, we have defined the following interface to assign a
rank to a solution (i.e, NSGA-II’s ranking):
```java
package org.uma.jmetal.util.solutionattribute;

import java.util.List;

/**
 * Ranks a list of solutions according to the dominance relationship
 *
 * @author Antonio J. Nebro <antonio@lcc.uma.es>
 */
public interface Ranking<S extends Solution<?>> extends SolutionAttribute<S, Integer>{
  public Ranking<S> computeRanking(List<S> solutionList) ;
  public List<S> getSubfront(int rank) ;
  public int getNumberOfSubfronts() ;
}
```

so that a client class (e.g., the `NSGAII` class) can merely use:
```java
Ranking ranking = computeRanking(jointPopulation);
```
This way, the solution attribute is managed internally by the class implementing the ranking and is hidden to the
metaheuristic.
