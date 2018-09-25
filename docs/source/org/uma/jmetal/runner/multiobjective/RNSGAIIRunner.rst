.. java:import:: org.uma.jmetal.algorithm Algorithm

.. java:import:: org.uma.jmetal.algorithm.multiobjective.rnsgaii RNSGAIIBuilder

.. java:import:: org.uma.jmetal.operator CrossoverOperator

.. java:import:: org.uma.jmetal.operator MutationOperator

.. java:import:: org.uma.jmetal.operator SelectionOperator

.. java:import:: org.uma.jmetal.operator.impl.crossover SBXCrossover

.. java:import:: org.uma.jmetal.operator.impl.mutation PolynomialMutation

.. java:import:: org.uma.jmetal.operator.impl.selection BinaryTournamentSelection

.. java:import:: org.uma.jmetal.problem Problem

.. java:import:: org.uma.jmetal.problem.multiobjective.zdt ZDT1

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.util AbstractAlgorithmRunner

.. java:import:: org.uma.jmetal.util AlgorithmRunner

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: org.uma.jmetal.util JMetalLogger

.. java:import:: org.uma.jmetal.util.comparator RankingAndCrowdingDistanceComparator

.. java:import:: java.io FileNotFoundException

.. java:import:: java.util ArrayList

.. java:import:: java.util List

RNSGAIIRunner
=============

.. java:package:: org.uma.jmetal.runner.multiobjective
   :noindex:

.. java:type:: public class RNSGAIIRunner extends AbstractAlgorithmRunner

   Class to configure and run the R-NSGA-II algorithm

   :author: Antonio J. Nebro , Cristobal Barba

Methods
-------
main
^^^^

.. java:method:: public static void main(String[] args) throws JMetalException, FileNotFoundException
   :outertype: RNSGAIIRunner

   :param args: Command line arguments.
   :throws JMetalException:
   :throws FileNotFoundException: Invoking command: java org.uma.jmetal.runner.multiobjective.RNSGAIIRunner problemName [referenceFront]

