.. java:import:: org.uma.jmetal.algorithm Algorithm

.. java:import:: org.uma.jmetal.algorithm.singleobjective.geneticalgorithm GeneticAlgorithmBuilder

.. java:import:: org.uma.jmetal.operator CrossoverOperator

.. java:import:: org.uma.jmetal.operator MutationOperator

.. java:import:: org.uma.jmetal.operator SelectionOperator

.. java:import:: org.uma.jmetal.operator.impl.crossover SBXCrossover

.. java:import:: org.uma.jmetal.operator.impl.mutation PolynomialMutation

.. java:import:: org.uma.jmetal.operator.impl.selection BinaryTournamentSelection

.. java:import:: org.uma.jmetal.problem DoubleProblem

.. java:import:: org.uma.jmetal.problem.singleobjective Sphere

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.util AlgorithmRunner

.. java:import:: org.uma.jmetal.util JMetalLogger

.. java:import:: org.uma.jmetal.util.fileoutput SolutionListOutput

.. java:import:: org.uma.jmetal.util.fileoutput.impl DefaultFileOutputContext

.. java:import:: java.util ArrayList

.. java:import:: java.util List

SteadyStateGeneticAlgorithmRunner
=================================

.. java:package:: org.uma.jmetal.runner.singleobjective
   :noindex:

.. java:type:: public class SteadyStateGeneticAlgorithmRunner

   Class to configure and run a steady-state genetic algorithm. The target problem is Sphere

   :author: Antonio J. Nebro

Methods
-------
main
^^^^

.. java:method:: public static void main(String[] args) throws Exception
   :outertype: SteadyStateGeneticAlgorithmRunner

   Usage: java org.uma.jmetal.runner.singleobjective.SteadyStateGeneticAlgorithmRunner

