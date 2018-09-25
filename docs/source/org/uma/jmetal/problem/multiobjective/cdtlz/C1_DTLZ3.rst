.. java:import:: org.uma.jmetal.problem ConstrainedProblem

.. java:import:: org.uma.jmetal.problem.multiobjective.dtlz DTLZ3

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.util.solutionattribute.impl NumberOfViolatedConstraints

.. java:import:: org.uma.jmetal.util.solutionattribute.impl OverallConstraintViolation

.. java:import:: java.util HashMap

.. java:import:: java.util Map

C1_DTLZ3
========

.. java:package:: org.uma.jmetal.problem.multiobjective.cdtlz
   :noindex:

.. java:type:: @SuppressWarnings public class C1_DTLZ3 extends DTLZ3 implements ConstrainedProblem<DoubleSolution>

   Problem C1-DTLZ3, defined in: Jain, H. and K. Deb. "An Evolutionary Many-Objective Optimization Algorithm Using Reference-Point-Based Nondominated Sorting Approach, Part II: Handling Constraints and Extending to an Adaptive Approach." EEE Transactions on Evolutionary Computation, 18(4):602-622, 2014.

   :author: Antonio J. Nebro

Fields
------
numberOfViolatedConstraints
^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:field:: public NumberOfViolatedConstraints<DoubleSolution> numberOfViolatedConstraints
   :outertype: C1_DTLZ3

overallConstraintViolationDegree
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:field:: public OverallConstraintViolation<DoubleSolution> overallConstraintViolationDegree
   :outertype: C1_DTLZ3

Constructors
------------
C1_DTLZ3
^^^^^^^^

.. java:constructor:: public C1_DTLZ3(int numberOfVariables, int numberOfObjectives)
   :outertype: C1_DTLZ3

   Constructor

   :param numberOfVariables:
   :param numberOfObjectives:

Methods
-------
evaluateConstraints
^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public void evaluateConstraints(DoubleSolution solution)
   :outertype: C1_DTLZ3

