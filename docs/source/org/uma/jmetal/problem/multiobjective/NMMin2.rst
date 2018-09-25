.. java:import:: org.uma.jmetal.problem.impl AbstractIntegerDoubleProblem

.. java:import:: org.uma.jmetal.solution IntegerDoubleSolution

.. java:import:: org.uma.jmetal.solution.impl DefaultIntegerDoubleSolution

.. java:import:: java.util ArrayList

.. java:import:: java.util List

NMMin2
======

.. java:package:: org.uma.jmetal.problem.multiobjective
   :noindex:

.. java:type:: @SuppressWarnings public class NMMin2 extends AbstractIntegerDoubleProblem<IntegerDoubleSolution>

   Created by Antonio J. Nebro on 18/09/14. Bi-objective problem for testing integer/double encoding. Objective 1: minimizing the distance to value N Objective 2: minimizing the distance to value M

Constructors
------------
NMMin2
^^^^^^

.. java:constructor:: public NMMin2()
   :outertype: NMMin2

NMMin2
^^^^^^

.. java:constructor:: public NMMin2(int numberOfIntegerVariables, int numberOfDoubleVariables, int n, int m, int lowerBound, int upperBound)
   :outertype: NMMin2

   Constructor

Methods
-------
createSolution
^^^^^^^^^^^^^^

.. java:method:: @Override public IntegerDoubleSolution createSolution()
   :outertype: NMMin2

evaluate
^^^^^^^^

.. java:method:: @Override public void evaluate(IntegerDoubleSolution solution)
   :outertype: NMMin2

   Evaluate() method

