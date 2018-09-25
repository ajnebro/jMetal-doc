.. java:import:: org.uma.jmetal.problem ConstrainedProblem

.. java:import:: org.uma.jmetal.problem.impl AbstractDoubleProblem

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.util.solutionattribute.impl NumberOfViolatedConstraints

.. java:import:: org.uma.jmetal.util.solutionattribute.impl OverallConstraintViolation

.. java:import:: java.util ArrayList

.. java:import:: java.util List

Tanaka
======

.. java:package:: org.uma.jmetal.problem.multiobjective
   :noindex:

.. java:type:: @SuppressWarnings public class Tanaka extends AbstractDoubleProblem implements ConstrainedProblem<DoubleSolution>

   Class representing problem Tanaka

Fields
------
numberOfViolatedConstraints
^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:field:: public NumberOfViolatedConstraints<DoubleSolution> numberOfViolatedConstraints
   :outertype: Tanaka

overallConstraintViolationDegree
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:field:: public OverallConstraintViolation<DoubleSolution> overallConstraintViolationDegree
   :outertype: Tanaka

Constructors
------------
Tanaka
^^^^^^

.. java:constructor:: public Tanaka()
   :outertype: Tanaka

   Constructor. Creates a default instance of the problem Tanaka

Methods
-------
evaluate
^^^^^^^^

.. java:method:: @Override public void evaluate(DoubleSolution solution)
   :outertype: Tanaka

evaluateConstraints
^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public void evaluateConstraints(DoubleSolution solution)
   :outertype: Tanaka

   EvaluateConstraints() method

