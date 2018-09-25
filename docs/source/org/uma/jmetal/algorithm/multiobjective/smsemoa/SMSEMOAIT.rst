.. java:import:: org.junit Test

.. java:import:: org.uma.jmetal.algorithm Algorithm

.. java:import:: org.uma.jmetal.operator CrossoverOperator

.. java:import:: org.uma.jmetal.operator MutationOperator

.. java:import:: org.uma.jmetal.operator.impl.crossover SBXCrossover

.. java:import:: org.uma.jmetal.operator.impl.mutation PolynomialMutation

.. java:import:: org.uma.jmetal.operator.impl.selection RandomSelection

.. java:import:: org.uma.jmetal.problem DoubleProblem

.. java:import:: org.uma.jmetal.problem.multiobjective.zdt ZDT1

.. java:import:: org.uma.jmetal.problem.multiobjective.zdt ZDT4

.. java:import:: org.uma.jmetal.qualityindicator QualityIndicator

.. java:import:: org.uma.jmetal.qualityindicator.impl Hypervolume

.. java:import:: org.uma.jmetal.qualityindicator.impl.hypervolume PISAHypervolume

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.util AlgorithmRunner

.. java:import:: java.util List

SMSEMOAIT
=========

.. java:package:: org.uma.jmetal.algorithm.multiobjective.smsemoa
   :noindex:

.. java:type:: public class SMSEMOAIT

Fields
------
algorithm
^^^^^^^^^

.. java:field::  Algorithm<List<DoubleSolution>> algorithm
   :outertype: SMSEMOAIT

Methods
-------
shouldTheAlgorithmReturnANumberOfSolutionsWhenSolvingASimpleProblem
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldTheAlgorithmReturnANumberOfSolutionsWhenSolvingASimpleProblem() throws Exception
   :outertype: SMSEMOAIT

shouldTheHypervolumeHaveAMinimumValue
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldTheHypervolumeHaveAMinimumValue() throws Exception
   :outertype: SMSEMOAIT

