## The `Problem` interface
To include a problem in jMetal, it must implement the `Problem` interface:

```java
package org.uma.jmetal.problem;

/**
 * Interface representing a multi-objective optimization problem
 *
 * @author Antonio J. Nebro <antonio@lcc.uma.es>
 *
 * @param <S> Encoding
 */
public interface Problem<S extends Solution<?>> extends Serializable {
  /* Getters */
  public int getNumberOfVariables() ;
  public int getNumberOfObjectives() ;
  public int getNumberOfConstraints() ;
  public String getName() ;

  /* Methods */
  public void evaluate(S solution) ;
  public S createSolution() ;
```

Every problem is characterized by the number of decision variables, the number of objective functions and the number of constraints, so getter methods for returning those values have to be defined. The genetic type `S` allows to determine the encoding of the solutions of the problem. This way, a problem must include a method for evaluating any solution of class `S` as well as providing a `createSolution()` method for creating a new solution. 

The `Solution` interface is generic, so jMetal 5 has a number of interfaces extending it to represent double (i.e., continous) problems, binary problems, etc. This way, the [`DoubleProblem`](https://github.com/jMetal/jMetal/blob/jmetal-5.0/jmetal-core/src/main/java/org/uma/jmetal/problem/DoubleProblem.java) interface is defined in this way:

```java
package org.uma.jmetal.problem;

/**
 * Interface representing continuous problems
 *
 * @author Antonio J. Nebro <antonio@lcc.uma.es>
 */
public interface DoubleProblem extends Problem<DoubleSolution> {
  Double getLowerBound(int index) ;
  Double getUpperBound(int index) ;
}
```
Problems implementing `DoubleProblem` only accept `DoubleSolution` objects, and methods for getting the lower and upper limits of each variable have to be implemented. jMetal 5 provides a default abstract class that implements `DoubleProblem` called [`AbstractDoubleProblem`](https://github.com/jMetal/jMetal/blob/jmetal-5.0/jmetal-core/src/main/java/org/uma/jmetal/problem/impl/AbstractDoubleProblem.java):
```java
package org.uma.jmetal.problem.impl;

public abstract class AbstractDoubleProblem extends AbstractGenericProblem<DoubleSolution>
  implements DoubleProblem {

  private List<Double> lowerLimit ;
  private List<Double> upperLimit ;

  /* Getters */
  @Override
  public Double getUpperBound(int index) {
    return upperLimit.get(index);
  }

  @Override
  public Double getLowerBound(int index) {
    return lowerLimit.get(index);
  }

  /* Setters */
  protected void setLowerLimit(List<Double> lowerLimit) {
    this.lowerLimit = lowerLimit;
  }

  protected void setUpperLimit(List<Double> upperLimit) {
    this.upperLimit = upperLimit;
  }

  @Override
  public DoubleSolution createSolution() {
    return new DefaultDoubleSolution(this)  ;
  }
}
```

As an example of double problem, we include next the implementation of the known [`Kursawe`](https://github.com/jMetal/jMetal/blob/jmetal-5.0/jmetal-problem/src/main/java/org/uma/jmetal/problem/multiobjective/Kursawe.java) problem:
```java
package org.uma.jmetal.problem.multiobjective;

/**
 * Class representing problem Kursawe
 */
public class Kursawe extends AbstractDoubleProblem {

  /**
   * Constructor.
   * Creates a default instance of the Kursawe problem.
   */
  public Kursawe() {
    // 3 variables by default
    this(3);
  }

  /**
   * Constructor.
   * Creates a new instance of the Kursawe problem.
   *
   * @param numberOfVariables Number of variables of the problem
   */
  public Kursawe(Integer numberOfVariables) {
    setNumberOfVariables(numberOfVariables);
    setNumberOfObjectives(2);
    setName("Kursawe");

    List<Double> lowerLimit = new ArrayList<>(getNumberOfVariables()) ;
    List<Double> upperLimit = new ArrayList<>(getNumberOfVariables()) ;

    for (int i = 0; i < getNumberOfVariables(); i++) {
      lowerLimit.add(-5.0);
      upperLimit.add(5.0);
    }

    setLowerLimit(lowerLimit);
    setUpperLimit(upperLimit);
  }

  /** Evaluate() method */
  public void evaluate(DoubleSolution solution){
    double aux, xi, xj;
    double[] fx = new double[getNumberOfObjectives()];
    double[] x = new double[getNumberOfVariables()];
    for (int i = 0; i < solution.getNumberOfVariables(); i++) {
      x[i] = solution.getVariableValue(i) ;
    }

    fx[0] = 0.0;
    for (int var = 0; var < solution.getNumberOfVariables() - 1; var++) {
      xi = x[var] * x[var];
      xj = x[var + 1] * x[var + 1];
      aux = (-0.2) * Math.sqrt(xi + xj);
      fx[0] += (-10.0) * Math.exp(aux);
    }

    fx[1] = 0.0;

    for (int var = 0; var < solution.getNumberOfVariables(); var++) {
      fx[1] += Math.pow(Math.abs(x[var]), 0.8) +
        5.0 * Math.sin(Math.pow(x[var], 3.0));
    }

    solution.setObjective(0, fx[0]);
    solution.setObjective(1, fx[1]);
  }
}
```

Similarly to the `DoubleProblem` interface and `AbstractDoubleProblem`, we can found `BinaryProblem` and `AbstractBinaryProblem`, `IntegerProblem` and `AbstractIntegerProblem`, etc. The packages related to defining and implementing problems are:
* [`org.uma.jmetal.problem` (module `jmetal-core`)](https://github.com/jMetal/jMetal/tree/jmetal-5.0/jmetal-core/src/main/java/org/uma/jmetal/problem): Interface definitions.
* [`org.uma.jmetal.problem.impl` (module `jmetal-core`)](https://github.com/jMetal/jMetal/tree/jmetal-5.0/jmetal-core/src/main/java/org/uma/jmetal/problem/impl): Default implementations.
* [`org.uma.jmetal.problem` (module `jmetal-problem`)](https://github.com/jMetal/jMetal/tree/jmetal-5.0/jmetal-problem/src/main/java/org/uma/jmetal/problem): Implemented problems.

### Constrained problems
There are two ways of dealing with constrained problems in jMetal 5. The first choice is to include the code to deal with constraint violation in the `evaluate()` method; the second one is to implement the [`ConstrainedProblem`](https://github.com/jMetal/jMetal/blob/jmetal-5.0/jmetal-core/src/main/java/org/uma/jmetal/problem/ConstrainedProblem.java) interface which includes a method for evaluating constraints:

```java
package org.uma.jmetal.problem;

/**
 * Interface representing problems having constraints
 *
 * @author Antonio J. Nebro <antonio@lcc.uma.es>
 */
public interface ConstrainedProblem<S extends Solution<?>> extends Problem<S> {

 /* Getters */
  public int getNumberOfConstraints() ;
	
  /* Methods */
  public void evaluateConstraints(S solution) ;
}
```
In jMetal 5 the default approach is the second one. The following code contains the implementation of the [`Tanaka`](https://github.com/jMetal/jMetal/blob/jmetal-5.0/jmetal-problem/src/main/java/org/uma/jmetal/problem/multiobjective/Tanaka.java) problem, which has two constraints:
```java
package org.uma.jmetal.problem.multiobjective;

/**
 * Class representing problem Tanaka
 */
public class Tanaka extends AbstractDoubleProblem implements ConstrainedProblem<DoubleSolution> {
  public OverallConstraintViolation<DoubleSolution> overallConstraintViolationDegree ;
  public NumberOfViolatedConstraints<DoubleSolution> numberOfViolatedConstraints ;

  /**
   * Constructor.
   * Creates a default instance of the problem Tanaka
   */
  public Tanaka() {
    setNumberOfVariables(2);
    setNumberOfObjectives(2);
    setNumberOfConstraints(2);
    setName("Tanaka") ;

    List<Double> lowerLimit = new ArrayList<>(getNumberOfVariables()) ;
    List<Double> upperLimit = new ArrayList<>(getNumberOfVariables()) ;

    for (int i = 0; i < getNumberOfVariables(); i++) {
      lowerLimit.add(10e-5);
      upperLimit.add(Math.PI);
    }

    setLowerLimit(lowerLimit);
    setUpperLimit(upperLimit);

    overallConstraintViolationDegree = new OverallConstraintViolation<DoubleSolution>() ;
    numberOfViolatedConstraints = new NumberOfViolatedConstraints<DoubleSolution>() ;
  }

  @Override
  public void evaluate(DoubleSolution solution)  {
    solution.setObjective(0, solution.getVariableValue(0));
    solution.setObjective(1, solution.getVariableValue(1));
  }

  /** EvaluateConstraints() method */
  @Override
  public void evaluateConstraints(DoubleSolution solution)  {
    double[] constraint = new double[this.getNumberOfConstraints()];

    double x1 = solution.getVariableValue(0) ;
    double x2 = solution.getVariableValue(1) ;

    constraint[0] = (x1 * x1 + x2 * x2 - 1.0 - 0.1 * Math.cos(16.0 * Math.atan(x1 / x2)));
    constraint[1] = -2.0 * ((x1 - 0.5) * (x1 - 0.5) + (x2 - 0.5) * (x2 - 0.5) - 0.5);

    double overallConstraintViolation = 0.0;
    int violatedConstraints = 0;
    for (int i = 0; i < getNumberOfConstraints(); i++) {
      if (constraint[i]<0.0){
        overallConstraintViolation+=constraint[i];
        violatedConstraints++;
      }
    }

    overallConstraintViolationDegree.setAttribute(solution, overallConstraintViolation);
    numberOfViolatedConstraints.setAttribute(solution, violatedConstraints);
  }
}

```
### Discusion
The inclusion of the `ConstrainedProblem` interface was motivated by the former jMetal versions, where every problem had the `evaluate()` and `evaluateConstraints()` methods. In the case of a non-constrained problem, `evaluateConstraints()` was implemented as an empty method. To avoid this violation of the [Interface Segregation Principle](https://en.wikipedia.org/wiki/Interface_segregation_principle), in jMetal 5 only those problems having side constraints need to evaluate constraints.

In the original jMetal, evaluating a solution needed two sentences:
```java
Problem problem ;
Solution solution ;
...
problem.evaluate(solution) ;
problem.evaluateContraints(solution) ;
```

Now a check has to be included to determine whether a problem has constraints or not:
```java
DoubleProblem problem ;
DoubleSolution solution ;

problem.evaluate(solution);
if (problem instanceof ConstrainedProblem) {
  ((ConstrainedProblem<DoubleSolution>) problem).evaluateConstraints(solutionn);
}
```
