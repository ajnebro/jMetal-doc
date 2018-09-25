.. java:import:: org.uma.jmetal.algorithm Algorithm

.. java:import:: org.uma.jmetal.algorithm.multiobjective.paes PAESBuilder

.. java:import:: org.uma.jmetal.operator MutationOperator

.. java:import:: org.uma.jmetal.operator.impl.mutation PolynomialMutation

.. java:import:: org.uma.jmetal.problem Problem

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: java.io FileNotFoundException

.. java:import:: java.util List

PAESRunner
==========

.. java:package:: org.uma.jmetal.runner.multiobjective
   :noindex:

.. java:type:: public class PAESRunner extends AbstractAlgorithmRunner

   Class for configuring and running the PAES algorithm

   :author: Antonio J. Nebro

Methods
-------
main
^^^^

.. java:method:: public static void main(String[] args) throws JMetalException, FileNotFoundException
   :outertype: PAESRunner

   :param args: Command line arguments.
   :throws SecurityException: Invoking command: java org.uma.jmetal.runner.multiobjective.PAESRunner problemName [referenceFront]

