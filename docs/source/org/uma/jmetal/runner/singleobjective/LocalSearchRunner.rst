.. java:import:: org.uma.jmetal.operator LocalSearchOperator

.. java:import:: org.uma.jmetal.operator MutationOperator

.. java:import:: org.uma.jmetal.operator.impl.localsearch BasicLocalSearch

.. java:import:: org.uma.jmetal.operator.impl.mutation BitFlipMutation

.. java:import:: org.uma.jmetal.problem BinaryProblem

.. java:import:: org.uma.jmetal.problem.singleobjective OneMax

.. java:import:: org.uma.jmetal.solution BinarySolution

.. java:import:: org.uma.jmetal.util JMetalLogger

.. java:import:: org.uma.jmetal.util.comparator DominanceComparator

.. java:import:: java.util Comparator

LocalSearchRunner
=================

.. java:package:: org.uma.jmetal.runner.singleobjective
   :noindex:

.. java:type:: public class LocalSearchRunner

   Class to configure and run a single objective local search. The target problem is OneMax.

   :author: Antonio J. Nebro

Methods
-------
main
^^^^

.. java:method:: public static void main(String[] args) throws Exception
   :outertype: LocalSearchRunner

   Usage: java org.uma.jmetal.runner.singleobjective.LocalSearchRunner

