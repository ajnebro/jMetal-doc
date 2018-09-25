.. java:import:: org.uma.jmetal.problem.impl AbstractIntegerProblem

.. java:import:: org.uma.jmetal.solution IntegerSolution

.. java:import:: java.util ArrayList

.. java:import:: java.util List

NIntegerMin
===========

.. java:package:: org.uma.jmetal.problem.singleobjective
   :noindex:

.. java:type:: @SuppressWarnings public class NIntegerMin extends AbstractIntegerProblem

   Created by Antonio J. Nebro on 03/07/14. Single objective problem for testing integer encoding. Objective: minimizing the distance to value N

Constructors
------------
NIntegerMin
^^^^^^^^^^^

.. java:constructor:: public NIntegerMin()
   :outertype: NIntegerMin

NIntegerMin
^^^^^^^^^^^

.. java:constructor:: public NIntegerMin(int numberOfVariables, int n, int lowerBound, int upperBound)
   :outertype: NIntegerMin

   Constructor

Methods
-------
evaluate
^^^^^^^^

.. java:method:: @Override public void evaluate(IntegerSolution solution)
   :outertype: NIntegerMin

   Evaluate() method

