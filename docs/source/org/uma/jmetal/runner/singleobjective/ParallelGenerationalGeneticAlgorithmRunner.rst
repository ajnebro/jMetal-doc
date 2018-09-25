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

.. java:import:: org.uma.jmetal.util.evaluator.impl MultithreadedSolutionListEvaluator

.. java:import:: org.uma.jmetal.util.fileoutput SolutionListOutput

.. java:import:: org.uma.jmetal.util.fileoutput.impl DefaultFileOutputContext

.. java:import:: java.util ArrayList

.. java:import:: java.util List

ParallelGenerationalGeneticAlgorithmRunner
==========================================

.. java:package:: org.uma.jmetal.runner.singleobjective
   :noindex:

.. java:type:: public class ParallelGenerationalGeneticAlgorithmRunner

   Class to configure and run a parallel (multithreaded) generational genetic algorithm. The number of cores is specified as an optional parameter. A default value is used is the parameter is not provided. The target problem is OneMax

   :author: Antonio J. Nebro

Methods
-------
main
^^^^

.. java:method:: public static void main(String[] args) throws Exception
   :outertype: ParallelGenerationalGeneticAlgorithmRunner

   Usage: java org.uma.jmetal.runner.singleobjective.ParallelGenerationalGeneticAlgorithmRunner [cores]

