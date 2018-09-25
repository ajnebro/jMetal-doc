.. java:import:: org.uma.jmetal.problem ConstrainedProblem

.. java:import:: org.uma.jmetal.problem.impl AbstractDoubleProblem

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.util.solutionattribute.impl NumberOfViolatedConstraints

.. java:import:: org.uma.jmetal.util.solutionattribute.impl OverallConstraintViolation

.. java:import:: java.util Arrays

.. java:import:: java.util List

ConstrEx
========

.. java:package:: org.uma.jmetal.problem.multiobjective
   :noindex:

.. java:type:: @SuppressWarnings public class ConstrEx extends AbstractDoubleProblem implements ConstrainedProblem<DoubleSolution>

   Class representing problem ConstrEx

Fields
------
numberOfViolatedConstraints
^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:field:: public NumberOfViolatedConstraints<DoubleSolution> numberOfViolatedConstraints
   :outertype: ConstrEx

overallConstraintViolationDegree
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:field:: public OverallConstraintViolation<DoubleSolution> overallConstraintViolationDegree
   :outertype: ConstrEx

Constructors
------------
ConstrEx
^^^^^^^^

.. java:constructor:: public ConstrEx()
   :outertype: ConstrEx

   Constructor Creates a default instance of the ConstrEx problem

Methods
-------
evaluate
^^^^^^^^

.. java:method:: @Override public void evaluate(DoubleSolution solution)
   :outertype: ConstrEx

   Evaluate() method

evaluateConstraints
^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public void evaluateConstraints(DoubleSolution solution)
   :outertype: ConstrEx

   EvaluateConstraints() method

