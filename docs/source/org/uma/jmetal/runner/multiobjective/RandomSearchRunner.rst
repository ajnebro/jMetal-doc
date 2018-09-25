.. java:import:: org.uma.jmetal.algorithm Algorithm

.. java:import:: org.uma.jmetal.algorithm.multiobjective.randomsearch RandomSearchBuilder

.. java:import:: org.uma.jmetal.problem Problem

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: java.io FileNotFoundException

.. java:import:: java.util List

RandomSearchRunner
==================

.. java:package:: org.uma.jmetal.runner.multiobjective
   :noindex:

.. java:type:: public class RandomSearchRunner extends AbstractAlgorithmRunner

   Class for configuring and running the random search algorithm

   :author: Antonio J. Nebro

Methods
-------
main
^^^^

.. java:method:: public static void main(String[] args) throws JMetalException, FileNotFoundException
   :outertype: RandomSearchRunner

   :param args: Command line arguments.
   :throws SecurityException: Invoking command: java org.uma.jmetal.runner.multiobjective.RandomSearchRunner problemName [referenceFront]

