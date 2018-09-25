.. java:import:: org.uma.jmetal.algorithm Algorithm

.. java:import:: org.uma.jmetal.algorithm.singleobjective.geneticalgorithm GeneticAlgorithmBuilder

.. java:import:: org.uma.jmetal.operator CrossoverOperator

.. java:import:: org.uma.jmetal.operator MutationOperator

.. java:import:: org.uma.jmetal.operator SelectionOperator

.. java:import:: org.uma.jmetal.operator.impl.crossover SinglePointCrossover

.. java:import:: org.uma.jmetal.operator.impl.mutation BitFlipMutation

.. java:import:: org.uma.jmetal.operator.impl.selection BinaryTournamentSelection

.. java:import:: org.uma.jmetal.problem BinaryProblem

.. java:import:: org.uma.jmetal.problem.singleobjective OneMax

.. java:import:: org.uma.jmetal.solution BinarySolution

.. java:import:: org.uma.jmetal.util AlgorithmRunner

.. java:import:: org.uma.jmetal.util JMetalLogger

.. java:import:: org.uma.jmetal.util.fileoutput SolutionListOutput

.. java:import:: org.uma.jmetal.util.fileoutput.impl DefaultFileOutputContext

.. java:import:: java.util ArrayList

.. java:import:: java.util List

SteadyStateGeneticAlgorithmBinaryEncodingRunner
===============================================

.. java:package:: org.uma.jmetal.runner.singleobjective
   :noindex:

.. java:type:: public class SteadyStateGeneticAlgorithmBinaryEncodingRunner

   Class to configure and run a steady-state genetic algorithm. The target problem is TSP

   :author: Antonio J. Nebro

Methods
-------
main
^^^^

.. java:method:: public static void main(String[] args) throws Exception
   :outertype: SteadyStateGeneticAlgorithmBinaryEncodingRunner

   Usage: java org.uma.jmetal.runner.singleobjective.SteadyStateGeneticAlgorithmBinaryEncodingRunner

