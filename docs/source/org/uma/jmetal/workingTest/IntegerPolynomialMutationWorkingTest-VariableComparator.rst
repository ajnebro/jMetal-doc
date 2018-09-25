.. java:import:: org.uma.jmetal.operator MutationOperator

.. java:import:: org.uma.jmetal.operator.impl.mutation IntegerPolynomialMutation

.. java:import:: org.uma.jmetal.problem IntegerProblem

.. java:import:: org.uma.jmetal.problem.singleobjective NIntegerMin

.. java:import:: org.uma.jmetal.solution IntegerSolution

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: org.uma.jmetal.util JMetalLogger

.. java:import:: java.util ArrayList

.. java:import:: java.util Collections

.. java:import:: java.util Comparator

.. java:import:: java.util List

IntegerPolynomialMutationWorkingTest.VariableComparator
=======================================================

.. java:package:: org.uma.jmetal.workingTest
   :noindex:

.. java:type:: public static class VariableComparator implements Comparator<IntegerSolution>
   :outertype: IntegerPolynomialMutationWorkingTest

Methods
-------
compare
^^^^^^^

.. java:method:: @Override public int compare(IntegerSolution solution1, IntegerSolution solution2)
   :outertype: IntegerPolynomialMutationWorkingTest.VariableComparator

   Compares two solutions according to the first variable value

   :param solution1: Object representing the first \ ``Solution``\ .
   :param solution2: Object representing the second \ ``Solution``\ .
   :return: -1, or 0, or 1 if o1 is less than, equal, or greater than o2, respectively.

