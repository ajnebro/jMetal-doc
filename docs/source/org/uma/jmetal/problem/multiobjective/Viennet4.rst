.. java:import:: org.uma.jmetal.problem ConstrainedProblem

.. java:import:: org.uma.jmetal.problem.impl AbstractDoubleProblem

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.util.solutionattribute.impl NumberOfViolatedConstraints

.. java:import:: org.uma.jmetal.util.solutionattribute.impl OverallConstraintViolation

.. java:import:: java.util ArrayList

.. java:import:: java.util List

Viennet4
========

.. java:package:: org.uma.jmetal.problem.multiobjective
   :noindex:

.. java:type:: @SuppressWarnings public class Viennet4 extends AbstractDoubleProblem implements ConstrainedProblem<DoubleSolution>

   Class representing problem Viennet4

Fields
------
numberOfViolatedConstraints
^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:field:: public NumberOfViolatedConstraints<DoubleSolution> numberOfViolatedConstraints
   :outertype: Viennet4

overallConstraintViolationDegree
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:field:: public OverallConstraintViolation<DoubleSolution> overallConstraintViolationDegree
   :outertype: Viennet4

Constructors
------------
Viennet4
^^^^^^^^

.. java:constructor:: public Viennet4()
   :outertype: Viennet4

   Constructor. Creates a default instance of the Viennet4 problem.

Methods
-------
evaluate
^^^^^^^^

.. java:method:: @Override public void evaluate(DoubleSolution solution)
   :outertype: Viennet4

   Evaluate() method

evaluateConstraints
^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public void evaluateConstraints(DoubleSolution solution)
   :outertype: Viennet4

   EvaluateConstraints() method

