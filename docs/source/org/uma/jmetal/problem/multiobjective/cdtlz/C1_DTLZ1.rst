.. java:import:: org.uma.jmetal.problem ConstrainedProblem

.. java:import:: org.uma.jmetal.problem.multiobjective.dtlz DTLZ1

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.util.solutionattribute.impl NumberOfViolatedConstraints

.. java:import:: org.uma.jmetal.util.solutionattribute.impl OverallConstraintViolation

C1_DTLZ1
========

.. java:package:: org.uma.jmetal.problem.multiobjective.cdtlz
   :noindex:

.. java:type:: @SuppressWarnings public class C1_DTLZ1 extends DTLZ1 implements ConstrainedProblem<DoubleSolution>

   Problem C1-DTLZ1, defined in: Jain, H. and K. Deb. "An Evolutionary Many-Objective Optimization Algorithm Using Reference-Point-Based Nondominated Sorting Approach, Part II: Handling Constraints and Extending to an Adaptive Approach." EEE Transactions on Evolutionary Computation, 18(4):602-622, 2014.

   :author: Antonio J. Nebro

Fields
------
numberOfViolatedConstraints
^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:field:: public NumberOfViolatedConstraints<DoubleSolution> numberOfViolatedConstraints
   :outertype: C1_DTLZ1

overallConstraintViolationDegree
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:field:: public OverallConstraintViolation<DoubleSolution> overallConstraintViolationDegree
   :outertype: C1_DTLZ1

Constructors
------------
C1_DTLZ1
^^^^^^^^

.. java:constructor:: public C1_DTLZ1(int numberOfVariables, int numberOfObjectives)
   :outertype: C1_DTLZ1

   Constructor

   :param numberOfVariables:
   :param numberOfObjectives:

Methods
-------
evaluateConstraints
^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public void evaluateConstraints(DoubleSolution solution)
   :outertype: C1_DTLZ1

