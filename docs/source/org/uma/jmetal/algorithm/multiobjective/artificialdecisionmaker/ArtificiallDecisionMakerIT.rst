.. java:import:: org.junit Ignore

.. java:import:: org.junit Test

.. java:import:: org.uma.jmetal.algorithm Algorithm

.. java:import:: org.uma.jmetal.algorithm InteractiveAlgorithm

.. java:import:: org.uma.jmetal.algorithm.multiobjective.wasfga WASFGA

.. java:import:: org.uma.jmetal.operator CrossoverOperator

.. java:import:: org.uma.jmetal.operator MutationOperator

.. java:import:: org.uma.jmetal.operator SelectionOperator

.. java:import:: org.uma.jmetal.operator.impl.crossover SBXCrossover

.. java:import:: org.uma.jmetal.operator.impl.mutation PolynomialMutation

.. java:import:: org.uma.jmetal.operator.impl.selection BinaryTournamentSelection

.. java:import:: org.uma.jmetal.problem Problem

.. java:import:: org.uma.jmetal.problem.multiobjective.dtlz DTLZ1

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.util AlgorithmRunner

.. java:import:: org.uma.jmetal.util.artificialdecisionmaker.impl ArtificialDecisionMakerDecisionTree

.. java:import:: org.uma.jmetal.util.artificialdecisionmaker.impl ArtificiallDecisionMakerBuilder

.. java:import:: org.uma.jmetal.util.comparator RankingAndCrowdingDistanceComparator

.. java:import:: org.uma.jmetal.util.evaluator.impl SequentialSolutionListEvaluator

.. java:import:: org.uma.jmetal.util.point.impl IdealPoint

.. java:import:: java.util ArrayList

.. java:import:: java.util List

.. java:import:: org.uma.jmetal.util.point.impl NadirPoint

ArtificiallDecisionMakerIT
==========================

.. java:package:: org.uma.jmetal.algorithm.multiobjective.artificialdecisionmaker
   :noindex:

.. java:type:: public class ArtificiallDecisionMakerIT

Fields
------
algorithm
^^^^^^^^^

.. java:field::  Algorithm<List<DoubleSolution>> algorithm
   :outertype: ArtificiallDecisionMakerIT

Methods
-------
shouldTheAlgorithmReturnANumberOfSolutionsWhenSolvingASimpleProblem
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Ignore @Test public void shouldTheAlgorithmReturnANumberOfSolutionsWhenSolvingASimpleProblem() throws Exception
   :outertype: ArtificiallDecisionMakerIT

