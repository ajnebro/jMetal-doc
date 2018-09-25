.. java:import:: org.uma.jmetal.problem ConstrainedProblem

.. java:import:: org.uma.jmetal.problem.impl AbstractDoubleProblem

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.util.solutionattribute.impl NumberOfViolatedConstraints

.. java:import:: org.uma.jmetal.util.solutionattribute.impl OverallConstraintViolation

.. java:import:: java.util Arrays

.. java:import:: java.util List

Water
=====

.. java:package:: org.uma.jmetal.problem.multiobjective
   :noindex:

.. java:type:: @SuppressWarnings public class Water extends AbstractDoubleProblem implements ConstrainedProblem<DoubleSolution>

   Class representing problem Water

Fields
------
LOWERLIMIT
^^^^^^^^^^

.. java:field:: public static final Double[] LOWERLIMIT
   :outertype: Water

UPPERLIMIT
^^^^^^^^^^

.. java:field:: public static final Double[] UPPERLIMIT
   :outertype: Water

numberOfViolatedConstraints
^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:field:: public NumberOfViolatedConstraints<DoubleSolution> numberOfViolatedConstraints
   :outertype: Water

overallConstraintViolationDegree
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:field:: public OverallConstraintViolation<DoubleSolution> overallConstraintViolationDegree
   :outertype: Water

Constructors
------------
Water
^^^^^

.. java:constructor:: public Water()
   :outertype: Water

   Constructor. Creates a default instance of the Water problem.

Methods
-------
evaluate
^^^^^^^^

.. java:method:: @Override public void evaluate(DoubleSolution solution)
   :outertype: Water

   Evaluate() method

evaluateConstraints
^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public void evaluateConstraints(DoubleSolution solution)
   :outertype: Water

   EvaluateConstraints() method

