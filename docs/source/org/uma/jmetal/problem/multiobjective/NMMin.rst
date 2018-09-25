.. java:import:: org.uma.jmetal.problem.impl AbstractIntegerProblem

.. java:import:: org.uma.jmetal.solution IntegerSolution

.. java:import:: java.util ArrayList

.. java:import:: java.util List

NMMin
=====

.. java:package:: org.uma.jmetal.problem.multiobjective
   :noindex:

.. java:type:: @SuppressWarnings public class NMMin extends AbstractIntegerProblem

   Created by Antonio J. Nebro on 03/07/14. Bi-objective problem for testing integer encoding. Objective 1: minimizing the distance to value N Objective 2: minimizing the distance to value M

Constructors
------------
NMMin
^^^^^

.. java:constructor:: public NMMin()
   :outertype: NMMin

NMMin
^^^^^

.. java:constructor:: public NMMin(int numberOfVariables, int n, int m, int lowerBound, int upperBound)
   :outertype: NMMin

   Constructor

Methods
-------
evaluate
^^^^^^^^

.. java:method:: @Override public void evaluate(IntegerSolution solution)
   :outertype: NMMin

   Evaluate() method

