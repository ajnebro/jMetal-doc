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

GenerationalGeneticAlgorithmDoubleEncodingRunner
================================================

.. java:package:: org.uma.jmetal.runner.singleobjective
   :noindex:

.. java:type:: public class GenerationalGeneticAlgorithmDoubleEncodingRunner

   Class to configure and run a generational genetic algorithm. The target problem is OneMax.

   :author: Antonio J. Nebro

Methods
-------
main
^^^^

.. java:method:: public static void main(String[] args) throws Exception
   :outertype: GenerationalGeneticAlgorithmDoubleEncodingRunner

   Usage: java org.uma.jmetal.runner.singleobjective.GenerationalGeneticAlgorithmDoubleEncodingRunner

