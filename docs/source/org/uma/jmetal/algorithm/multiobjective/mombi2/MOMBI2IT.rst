.. java:import:: org.junit Test

.. java:import:: org.uma.jmetal.algorithm Algorithm

.. java:import:: org.uma.jmetal.algorithm.multiobjective.mombi MOMBI2

.. java:import:: org.uma.jmetal.operator CrossoverOperator

.. java:import:: org.uma.jmetal.operator MutationOperator

.. java:import:: org.uma.jmetal.operator SelectionOperator

.. java:import:: org.uma.jmetal.operator.impl.crossover SBXCrossover

.. java:import:: org.uma.jmetal.operator.impl.mutation PolynomialMutation

.. java:import:: org.uma.jmetal.operator.impl.selection BinaryTournamentSelection

.. java:import:: org.uma.jmetal.problem.multiobjective.dtlz DTLZ1

.. java:import:: org.uma.jmetal.qualityindicator QualityIndicator

.. java:import:: org.uma.jmetal.qualityindicator.impl.hypervolume PISAHypervolume

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.util AlgorithmRunner

.. java:import:: org.uma.jmetal.util.comparator RankingAndCrowdingDistanceComparator

.. java:import:: org.uma.jmetal.util.evaluator.impl SequentialSolutionListEvaluator

.. java:import:: org.uma.jmetal.util.pseudorandom JMetalRandom

.. java:import:: java.util List

MOMBI2IT
========

.. java:package:: org.uma.jmetal.algorithm.multiobjective.mombi2
   :noindex:

.. java:type:: public class MOMBI2IT

Fields
------
algorithm
^^^^^^^^^

.. java:field::  Algorithm<List<DoubleSolution>> algorithm
   :outertype: MOMBI2IT

Methods
-------
shouldTheAlgorithmReturnANumberOfSolutionsWhenSolvingASimpleProblem
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldTheAlgorithmReturnANumberOfSolutionsWhenSolvingASimpleProblem() throws Exception
   :outertype: MOMBI2IT

shouldTheHypervolumeHaveAMininumValue
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldTheHypervolumeHaveAMininumValue() throws Exception
   :outertype: MOMBI2IT

