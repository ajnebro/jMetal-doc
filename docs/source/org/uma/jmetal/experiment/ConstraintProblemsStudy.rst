.. java:import:: org.uma.jmetal.algorithm Algorithm

.. java:import:: org.uma.jmetal.algorithm.multiobjective.gde3 GDE3Builder

.. java:import:: org.uma.jmetal.algorithm.multiobjective.mocell MOCellBuilder

.. java:import:: org.uma.jmetal.algorithm.multiobjective.nsgaii NSGAIIBuilder

.. java:import:: org.uma.jmetal.algorithm.multiobjective.smpso SMPSOBuilder

.. java:import:: org.uma.jmetal.algorithm.multiobjective.spea2 SPEA2Builder

.. java:import:: org.uma.jmetal.operator.impl.crossover DifferentialEvolutionCrossover

.. java:import:: org.uma.jmetal.operator.impl.crossover SBXCrossover

.. java:import:: org.uma.jmetal.operator.impl.mutation PolynomialMutation

.. java:import:: org.uma.jmetal.operator.impl.selection BinaryTournamentSelection

.. java:import:: org.uma.jmetal.operator.impl.selection DifferentialEvolutionSelection

.. java:import:: org.uma.jmetal.problem DoubleProblem

.. java:import:: org.uma.jmetal.problem Problem

.. java:import:: org.uma.jmetal.qualityindicator.impl Epsilon

.. java:import:: org.uma.jmetal.qualityindicator.impl InvertedGenerationalDistancePlus

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

ConstraintProblemsStudy
=======================

.. java:package:: org.uma.jmetal.experiment
   :noindex:

.. java:type:: public class ConstraintProblemsStudy

   Example of experimental study based on solving the unconstrained problems included in jMetal. This experiment assumes that the reference Pareto front are known and that, given a problem named P, there is a corresponding file called P.pf containing its corresponding Pareto front. If this is not the case, please refer to class \ :java:ref:`DTLZStudy`\  to see an example of how to explicitly indicate the name of those files. Six quality indicators are used for performance assessment. The steps to carry out the experiment are: 1. Configure the experiment 2. Execute the algorithms 3. Generate the reference Pareto fronts 4. Compute the quality indicators 5. Generate Latex tables reporting means and medians 6. Generate Latex tables with the result of applying the Wilcoxon Rank Sum Test 7. Generate Latex tables with the ranking obtained by applying the Friedman test 8. Generate R scripts to obtain boxplots

   :author: Antonio J. Nebro

Methods
-------
configureAlgorithmList
^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: static List<ExperimentAlgorithm<DoubleSolution, List<DoubleSolution>>> configureAlgorithmList(List<ExperimentProblem<DoubleSolution>> problemList)
   :outertype: ConstraintProblemsStudy

   The algorithm list is composed of pairs \ :java:ref:`Algorithm`\  + \ :java:ref:`Problem`\  which form part of a \ :java:ref:`ExperimentAlgorithm`\ , which is a decorator for class \ :java:ref:`Algorithm`\ . The \ :java:ref:`ExperimentAlgorithm`\  has an optional tag component, that can be set as it is shown in this example, where four variants of a same algorithm are defined.

main
^^^^

.. java:method:: public static void main(String[] args) throws IOException
   :outertype: ConstraintProblemsStudy

