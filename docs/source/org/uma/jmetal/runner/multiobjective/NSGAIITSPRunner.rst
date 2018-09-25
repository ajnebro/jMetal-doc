.. java:import:: org.uma.jmetal.algorithm Algorithm

.. java:import:: org.uma.jmetal.algorithm.multiobjective.nsgaii NSGAIIBuilder

.. java:import:: org.uma.jmetal.operator CrossoverOperator

.. java:import:: org.uma.jmetal.operator MutationOperator

.. java:import:: org.uma.jmetal.operator SelectionOperator

.. java:import:: org.uma.jmetal.operator.impl.crossover PMXCrossover

.. java:import:: org.uma.jmetal.operator.impl.mutation PermutationSwapMutation

.. java:import:: org.uma.jmetal.operator.impl.selection BinaryTournamentSelection

.. java:import:: org.uma.jmetal.problem PermutationProblem

.. java:import:: org.uma.jmetal.problem.multiobjective MultiobjectiveTSP

.. java:import:: org.uma.jmetal.solution PermutationSolution

.. java:import:: org.uma.jmetal.util AbstractAlgorithmRunner

.. java:import:: org.uma.jmetal.util AlgorithmRunner

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: org.uma.jmetal.util JMetalLogger

.. java:import:: org.uma.jmetal.util.comparator RankingAndCrowdingDistanceComparator

.. java:import:: org.uma.jmetal.util.fileoutput SolutionListOutput

.. java:import:: org.uma.jmetal.util.fileoutput.impl DefaultFileOutputContext

.. java:import:: org.uma.jmetal.util.pseudorandom JMetalRandom

.. java:import:: java.io IOException

.. java:import:: java.util List

NSGAIITSPRunner
===============

.. java:package:: org.uma.jmetal.runner.multiobjective
   :noindex:

.. java:type:: public class NSGAIITSPRunner extends AbstractAlgorithmRunner

   Class for configuring and running the NSGA-II algorithm to solve the bi-objective TSP

   :author: Antonio J. Nebro

Methods
-------
main
^^^^

.. java:method:: public static void main(String[] args) throws JMetalException, IOException
   :outertype: NSGAIITSPRunner

   :param args: Command line arguments.
   :throws java.io.IOException:
   :throws SecurityException:
   :throws ClassNotFoundException: Invoking command: java org.uma.jmetal.runner.multiobjective.NSGAIITSPRunner problemName [referenceFront]

