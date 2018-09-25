.. java:import:: org.uma.jmetal.problem ConstrainedProblem

.. java:import:: org.uma.jmetal.problem.multiobjective.dtlz DTLZ2

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.util.solutionattribute.impl NumberOfViolatedConstraints

.. java:import:: org.uma.jmetal.util.solutionattribute.impl OverallConstraintViolation

.. java:import:: java.util HashMap

.. java:import:: java.util Map

ConvexC2_DTLZ2
==============

.. java:package:: org.uma.jmetal.problem.multiobjective.cdtlz
   :noindex:

.. java:type:: @SuppressWarnings public class ConvexC2_DTLZ2 extends DTLZ2 implements ConstrainedProblem<DoubleSolution>

   Problem ConvexC2-DTLZ2, defined in: Jain, H. and K. Deb. "An Evolutionary Many-Objective Optimization Algorithm Using Reference-Point-Based Nondominated Sorting Approach, Part II: Handling Constraints and Extending to an Adaptive Approach." EEE Transactions on Evolutionary Computation, 18(4):602-622, 2014.

   :author: Antonio J. Nebro

Fields
------
numberOfViolatedConstraints
^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:field:: public NumberOfViolatedConstraints<DoubleSolution> numberOfViolatedConstraints
   :outertype: ConvexC2_DTLZ2

overallConstraintViolationDegree
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:field:: public OverallConstraintViolation<DoubleSolution> overallConstraintViolationDegree
   :outertype: ConvexC2_DTLZ2

Constructors
------------
ConvexC2_DTLZ2
^^^^^^^^^^^^^^

.. java:constructor:: public ConvexC2_DTLZ2(int numberOfVariables, int numberOfObjectives)
   :outertype: ConvexC2_DTLZ2

   Constructor

   :param numberOfVariables:
   :param numberOfObjectives:

Methods
-------
evaluateConstraints
^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public void evaluateConstraints(DoubleSolution solution)
   :outertype: ConvexC2_DTLZ2

