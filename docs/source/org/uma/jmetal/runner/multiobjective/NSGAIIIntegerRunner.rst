.. java:import:: org.uma.jmetal.algorithm Algorithm

.. java:import:: org.uma.jmetal.algorithm.multiobjective.nsgaii NSGAIIBuilder

.. java:import:: org.uma.jmetal.operator CrossoverOperator

.. java:import:: org.uma.jmetal.operator MutationOperator

.. java:import:: org.uma.jmetal.operator SelectionOperator

.. java:import:: org.uma.jmetal.operator.impl.crossover IntegerSBXCrossover

.. java:import:: org.uma.jmetal.operator.impl.mutation IntegerPolynomialMutation

.. java:import:: org.uma.jmetal.operator.impl.selection BinaryTournamentSelection

.. java:import:: org.uma.jmetal.problem Problem

.. java:import:: org.uma.jmetal.solution IntegerSolution

.. java:import:: org.uma.jmetal.util AbstractAlgorithmRunner

.. java:import:: org.uma.jmetal.util AlgorithmRunner

.. java:import:: org.uma.jmetal.util JMetalLogger

.. java:import:: org.uma.jmetal.util ProblemUtils

.. java:import:: java.io FileNotFoundException

.. java:import:: java.util List

NSGAIIIntegerRunner
===================

.. java:package:: org.uma.jmetal.runner.multiobjective
   :noindex:

.. java:type:: public class NSGAIIIntegerRunner extends AbstractAlgorithmRunner

   Class for configuring and running the NSGA-II algorithm (integer encoding)

   :author: Antonio J. Nebro

Methods
-------
main
^^^^

.. java:method:: public static void main(String[] args) throws FileNotFoundException
   :outertype: NSGAIIIntegerRunner

   :param args: Command line arguments.
   :throws org.uma.jmetal.util.JMetalException:
   :throws java.io.IOException:
   :throws SecurityException:
   :throws ClassNotFoundException: Invoking command: java org.uma.jmetal.runner.multiobjective.NSGAIIIntegerRunner problemName [referenceFront]

