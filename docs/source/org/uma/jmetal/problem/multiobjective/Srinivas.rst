.. java:import:: org.uma.jmetal.problem ConstrainedProblem

.. java:import:: org.uma.jmetal.problem.impl AbstractDoubleProblem

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.util.solutionattribute.impl NumberOfViolatedConstraints

.. java:import:: org.uma.jmetal.util.solutionattribute.impl OverallConstraintViolation

.. java:import:: java.util ArrayList

.. java:import:: java.util List

Srinivas
========

.. java:package:: org.uma.jmetal.problem.multiobjective
   :noindex:

.. java:type:: @SuppressWarnings public class Srinivas extends AbstractDoubleProblem implements ConstrainedProblem<DoubleSolution>

   Class representing problem Srinivas

Fields
------
numberOfViolatedConstraints
^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:field:: public NumberOfViolatedConstraints<DoubleSolution> numberOfViolatedConstraints
   :outertype: Srinivas

overallConstraintViolationDegree
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:field:: public OverallConstraintViolation<DoubleSolution> overallConstraintViolationDegree
   :outertype: Srinivas

Constructors
------------
Srinivas
^^^^^^^^

.. java:constructor:: public Srinivas()
   :outertype: Srinivas

   Constructor

Methods
-------
evaluate
^^^^^^^^

.. java:method:: @Override public void evaluate(DoubleSolution solution)
   :outertype: Srinivas

   Evaluate() method

evaluateConstraints
^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public void evaluateConstraints(DoubleSolution solution)
   :outertype: Srinivas

   EvaluateConstraints() method

