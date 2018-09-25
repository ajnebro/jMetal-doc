.. java:import:: org.uma.jmetal.problem ConstrainedProblem

.. java:import:: org.uma.jmetal.problem.multiobjective.dtlz DTLZ4

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.util.solutionattribute.impl NumberOfViolatedConstraints

.. java:import:: org.uma.jmetal.util.solutionattribute.impl OverallConstraintViolation

C3_DTLZ4
========

.. java:package:: org.uma.jmetal.problem.multiobjective.cdtlz
   :noindex:

.. java:type:: @SuppressWarnings public class C3_DTLZ4 extends DTLZ4 implements ConstrainedProblem<DoubleSolution>

   Problem C3-DTLZ4, defined in: Jain, H. and K. Deb. "An Evolutionary Many-Objective Optimization Algorithm Using Reference-Point-Based Nondominated Sorting Approach, Part II: Handling Constraints and Extending to an Adaptive Approach." EEE Transactions on Evolutionary Computation, 18(4):602-622, 2014.

   :author: Antonio J. Nebro

Fields
------
numberOfViolatedConstraints
^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:field:: public NumberOfViolatedConstraints<DoubleSolution> numberOfViolatedConstraints
   :outertype: C3_DTLZ4

overallConstraintViolationDegree
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:field:: public OverallConstraintViolation<DoubleSolution> overallConstraintViolationDegree
   :outertype: C3_DTLZ4

Constructors
------------
C3_DTLZ4
^^^^^^^^

.. java:constructor:: public C3_DTLZ4(int numberOfVariables, int numberOfObjectives, int numberOfConstraints)
   :outertype: C3_DTLZ4

   Constructor

   :param numberOfVariables:
   :param numberOfObjectives:

Methods
-------
evaluateConstraints
^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public void evaluateConstraints(DoubleSolution solution)
   :outertype: C3_DTLZ4

