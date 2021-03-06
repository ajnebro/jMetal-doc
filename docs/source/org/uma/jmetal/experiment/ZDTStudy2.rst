.. java:import:: org.uma.jmetal.algorithm Algorithm

.. java:import:: org.uma.jmetal.algorithm.multiobjective.moead AbstractMOEAD

.. java:import:: org.uma.jmetal.algorithm.multiobjective.moead MOEADBuilder

.. java:import:: org.uma.jmetal.algorithm.multiobjective.nsgaii NSGAIIBuilder

.. java:import:: org.uma.jmetal.algorithm.multiobjective.smpso SMPSOBuilder

.. java:import:: org.uma.jmetal.algorithm.multiobjective.spea2 SPEA2Builder

.. java:import:: org.uma.jmetal.operator.impl.crossover DifferentialEvolutionCrossover

.. java:import:: org.uma.jmetal.operator.impl.crossover SBXCrossover

.. java:import:: org.uma.jmetal.operator.impl.mutation PolynomialMutation

.. java:import:: org.uma.jmetal.problem DoubleProblem

.. java:import:: org.uma.jmetal.problem Problem

.. java:import:: org.uma.jmetal.qualityindicator.impl.hypervolume PISAHypervolume

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: org.uma.jmetal.util.archive.impl CrowdingDistanceArchive

.. java:import:: org.uma.jmetal.util.evaluator.impl SequentialSolutionListEvaluator

.. java:import:: org.uma.jmetal.util.experiment Experiment

.. java:import:: org.uma.jmetal.util.experiment ExperimentBuilder

.. java:import:: org.uma.jmetal.util.experiment.util ExperimentAlgorithm

.. java:import:: org.uma.jmetal.util.experiment.util ExperimentProblem

.. java:import:: java.io IOException

.. java:import:: java.util ArrayList

.. java:import:: java.util Arrays

.. java:import:: java.util List

ZDTStudy2
=========

.. java:package:: org.uma.jmetal.experiment
   :noindex:

.. java:type:: public class ZDTStudy2

   Example of experimental study based on solving the ZDT problems with algorithms NSGAII, MOEA/D, and SMPSO This experiment assumes that the reference Pareto front are not known, so the names of files containing them and the directory where they are located must be specified. Six quality indicators are used for performance assessment. The steps to carry out the experiment are: 1. Configure the experiment 2. Execute the algorithms 3. Generate the reference Pareto fronts 4. Compute que quality indicators 5. Generate Latex tables reporting means and medians 6. Generate Latex tables with the result of applying the Wilcoxon Rank Sum Test 7. Generate R scripts to obtain boxplots

   :author: Antonio J. Nebro

Methods
-------
configureAlgorithmList
^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: static List<ExperimentAlgorithm<DoubleSolution, List<DoubleSolution>>> configureAlgorithmList(List<ExperimentProblem<DoubleSolution>> problemList)
   :outertype: ZDTStudy2

   The algorithm list is composed of pairs \ :java:ref:`Algorithm`\  + \ :java:ref:`Problem`\  which form part of a \ :java:ref:`ExperimentAlgorithm`\ , which is a decorator for class \ :java:ref:`Algorithm`\ .

main
^^^^

.. java:method:: public static void main(String[] args) throws IOException
   :outertype: ZDTStudy2

