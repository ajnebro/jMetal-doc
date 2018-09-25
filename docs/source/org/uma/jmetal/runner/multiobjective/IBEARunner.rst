.. java:import:: org.uma.jmetal.algorithm.multiobjective.ibea IBEA

.. java:import:: org.uma.jmetal.algorithm.multiobjective.ibea IBEABuilder

.. java:import:: org.uma.jmetal.operator CrossoverOperator

.. java:import:: org.uma.jmetal.operator MutationOperator

.. java:import:: org.uma.jmetal.operator SelectionOperator

.. java:import:: org.uma.jmetal.operator.impl.crossover SBXCrossover

.. java:import:: org.uma.jmetal.operator.impl.mutation PolynomialMutation

.. java:import:: org.uma.jmetal.operator.impl.selection BinaryTournamentSelection

.. java:import:: org.uma.jmetal.problem Problem

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.util AbstractAlgorithmRunner

.. java:import:: org.uma.jmetal.util AlgorithmRunner

.. java:import:: org.uma.jmetal.util JMetalLogger

.. java:import:: org.uma.jmetal.util ProblemUtils

.. java:import:: java.util List

IBEARunner
==========

.. java:package:: org.uma.jmetal.runner.multiobjective
   :noindex:

.. java:type:: public class IBEARunner extends AbstractAlgorithmRunner

   Class for configuring and running the IBEA algorithm

   :author: Antonio J. Nebro

Methods
-------
main
^^^^

.. java:method:: public static void main(String[] args) throws Exception
   :outertype: IBEARunner

   :param args: Command line arguments.
   :throws java.io.IOException:
   :throws SecurityException:
   :throws ClassNotFoundException: Invoking command: java org.uma.jmetal.runner.multiobjective.IBEARunner problemName [referenceFront]

