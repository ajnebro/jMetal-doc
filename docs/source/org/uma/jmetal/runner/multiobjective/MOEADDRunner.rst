.. java:import:: org.uma.jmetal.algorithm Algorithm

.. java:import:: org.uma.jmetal.algorithm.multiobjective.moead AbstractMOEAD

.. java:import:: org.uma.jmetal.algorithm.multiobjective.moead MOEADBuilder

.. java:import:: org.uma.jmetal.operator CrossoverOperator

.. java:import:: org.uma.jmetal.operator MutationOperator

.. java:import:: org.uma.jmetal.operator.impl.crossover SBXCrossover

.. java:import:: org.uma.jmetal.operator.impl.mutation PolynomialMutation

.. java:import:: org.uma.jmetal.problem DoubleProblem

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.util AbstractAlgorithmRunner

.. java:import:: org.uma.jmetal.util AlgorithmRunner

.. java:import:: org.uma.jmetal.util JMetalLogger

.. java:import:: org.uma.jmetal.util ProblemUtils

.. java:import:: java.io FileNotFoundException

.. java:import:: java.util List

MOEADDRunner
============

.. java:package:: org.uma.jmetal.runner.multiobjective
   :noindex:

.. java:type:: public class MOEADDRunner extends AbstractAlgorithmRunner

   Class for configuring and running the MOEA/DD algorithm

   :author:

Methods
-------
main
^^^^

.. java:method:: public static void main(String[] args) throws FileNotFoundException
   :outertype: MOEADDRunner

   :param args: Command line arguments.
   :throws SecurityException: Invoking command: java org.uma.jmetal.runner.multiobjective.MOEADRunner problemName [referenceFront]

