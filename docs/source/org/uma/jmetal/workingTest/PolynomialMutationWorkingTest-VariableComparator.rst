.. java:import:: org.uma.jmetal.operator MutationOperator

.. java:import:: org.uma.jmetal.operator.impl.mutation PolynomialMutation

.. java:import:: org.uma.jmetal.problem DoubleProblem

.. java:import:: org.uma.jmetal.problem.singleobjective Sphere

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: java.util ArrayList

.. java:import:: java.util Collections

.. java:import:: java.util Comparator

.. java:import:: java.util List

PolynomialMutationWorkingTest.VariableComparator
================================================

.. java:package:: org.uma.jmetal.workingTest
   :noindex:

.. java:type:: public static class VariableComparator implements Comparator<DoubleSolution>
   :outertype: PolynomialMutationWorkingTest

Methods
-------
compare
^^^^^^^

.. java:method:: @Override public int compare(DoubleSolution solution1, DoubleSolution solution2)
   :outertype: PolynomialMutationWorkingTest.VariableComparator

   Compares two solutions according to the first variable value

   :param solution1: Object representing the first \ ``Solution``\ .
   :param solution2: Object representing the second \ ``Solution``\ .
   :return: -1, or 0, or 1 if o1 is less than, equal, or greater than o2, respectively.

