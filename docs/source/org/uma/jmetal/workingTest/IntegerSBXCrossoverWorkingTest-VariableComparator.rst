.. java:import:: org.uma.jmetal.operator CrossoverOperator

.. java:import:: org.uma.jmetal.operator.impl.crossover IntegerSBXCrossover

.. java:import:: org.uma.jmetal.problem IntegerProblem

.. java:import:: org.uma.jmetal.problem.multiobjective NMMin

.. java:import:: org.uma.jmetal.solution IntegerSolution

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: org.uma.jmetal.util.fileoutput SolutionListOutput

.. java:import:: org.uma.jmetal.util.fileoutput.impl DefaultFileOutputContext

IntegerSBXCrossoverWorkingTest.VariableComparator
=================================================

.. java:package:: org.uma.jmetal.workingTest
   :noindex:

.. java:type:: public static class VariableComparator implements Comparator<IntegerSolution>
   :outertype: IntegerSBXCrossoverWorkingTest

Methods
-------
compare
^^^^^^^

.. java:method:: @Override public int compare(IntegerSolution solution1, IntegerSolution solution2)
   :outertype: IntegerSBXCrossoverWorkingTest.VariableComparator

   Compares two solutions according to the first variable value

   :param solution1: Object representing the first \ ``Solution``\ .
   :param solution2: Object representing the second \ ``Solution``\ .
   :return: -1, or 0, or 1 if o1 is less than, equal, or greater than o2, respectively.

