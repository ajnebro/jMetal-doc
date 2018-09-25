.. java:import:: org.uma.jmetal.algorithm Algorithm

.. java:import:: org.uma.jmetal.algorithm.multiobjective.espea ESPEABuilder

.. java:import:: org.uma.jmetal.algorithm.multiobjective.espea.util EnergyArchive.ReplacementStrategy

.. java:import:: org.uma.jmetal.operator CrossoverOperator

.. java:import:: org.uma.jmetal.operator MutationOperator

.. java:import:: org.uma.jmetal.operator.impl.crossover SBXCrossover

.. java:import:: org.uma.jmetal.operator.impl.mutation PolynomialMutation

.. java:import:: org.uma.jmetal.problem Problem

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: java.io FileNotFoundException

.. java:import:: java.util List

ESPEARunner
===========

.. java:package:: org.uma.jmetal.runner.multiobjective
   :noindex:

.. java:type:: public class ESPEARunner extends AbstractAlgorithmRunner

   Class to configure and run the ESPEA algorithm

   :author: Marlon Braun

Methods
-------
main
^^^^

.. java:method:: public static void main(String[] args) throws JMetalException, FileNotFoundException
   :outertype: ESPEARunner

   :param args: Command line arguments.
   :throws FileNotFoundException: Invoking command: java org.uma.jmetal.runner.multiobjective.ESPEARunner problemName [referenceFront]

