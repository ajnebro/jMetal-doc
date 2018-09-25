.. java:import:: org.uma.jmetal.algorithm Algorithm

.. java:import:: org.uma.jmetal.algorithm.multiobjective.mocell MOCellBuilder

.. java:import:: org.uma.jmetal.algorithm.multiobjective.mochc MOCHCBuilder

.. java:import:: org.uma.jmetal.algorithm.multiobjective.nsgaii NSGAIIBuilder

.. java:import:: org.uma.jmetal.algorithm.multiobjective.spea2 SPEA2Builder

.. java:import:: org.uma.jmetal.operator CrossoverOperator

.. java:import:: org.uma.jmetal.operator MutationOperator

.. java:import:: org.uma.jmetal.operator SelectionOperator

.. java:import:: org.uma.jmetal.operator.impl.crossover HUXCrossover

.. java:import:: org.uma.jmetal.operator.impl.crossover SinglePointCrossover

.. java:import:: org.uma.jmetal.operator.impl.mutation BitFlipMutation

.. java:import:: org.uma.jmetal.operator.impl.selection RandomSelection

.. java:import:: org.uma.jmetal.operator.impl.selection RankingAndCrowdingSelection

.. java:import:: org.uma.jmetal.problem BinaryProblem

.. java:import:: org.uma.jmetal.problem Problem

.. java:import:: org.uma.jmetal.problem.multiobjective OneZeroMax

.. java:import:: org.uma.jmetal.problem.multiobjective.zdt ZDT5

.. java:import:: org.uma.jmetal.qualityindicator.impl.hypervolume PISAHypervolume

.. java:import:: org.uma.jmetal.solution BinarySolution

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: org.uma.jmetal.util.evaluator.impl SequentialSolutionListEvaluator

.. java:import:: org.uma.jmetal.util.experiment Experiment

.. java:import:: org.uma.jmetal.util.experiment ExperimentBuilder

.. java:import:: org.uma.jmetal.util.experiment.util ExperimentAlgorithm

.. java:import:: org.uma.jmetal.util.experiment.util ExperimentProblem

.. java:import:: java.io IOException

.. java:import:: java.util ArrayList

.. java:import:: java.util Arrays

.. java:import:: java.util List

BinaryProblemsStudy
===================

.. java:package:: org.uma.jmetal.experiment
   :noindex:

.. java:type:: public class BinaryProblemsStudy

   Example of experimental study based on solving two binary problems with four algorithms: NSGAII, SPEA2, MOCell, and MOCHC This experiment assumes that the reference Pareto front are not known, so the must be produced. Six quality indicators are used for performance assessment. The steps to carry out the experiment are: 1. Configure the experiment 2. Execute the algorithms 3. Generate the reference Pareto fronts 4. Compute que quality indicators 5. Generate Latex tables reporting means and medians 6. Generate Latex tables with the result of applying the Wilcoxon Rank Sum Test 7. Generate Latex tables with the ranking obtained by applying the Friedman test 8. Generate R scripts to obtain boxplots

   :author: Antonio J. Nebro

Methods
-------
configureAlgorithmList
^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: static List<ExperimentAlgorithm<BinarySolution, List<BinarySolution>>> configureAlgorithmList(List<ExperimentProblem<BinarySolution>> problemList)
   :outertype: BinaryProblemsStudy

   The algorithm list is composed of pairs \ :java:ref:`Algorithm`\  + \ :java:ref:`Problem`\  which form part of a \ :java:ref:`ExperimentAlgorithm`\ , which is a decorator for class \ :java:ref:`Algorithm`\ .

main
^^^^

.. java:method:: public static void main(String[] args) throws IOException
   :outertype: BinaryProblemsStudy

