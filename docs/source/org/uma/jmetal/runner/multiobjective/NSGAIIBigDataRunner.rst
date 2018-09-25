.. java:import:: org.uma.jmetal.algorithm Algorithm

.. java:import:: org.uma.jmetal.algorithm.multiobjective.nsgaii NSGAIIBuilder

.. java:import:: org.uma.jmetal.operator CrossoverOperator

.. java:import:: org.uma.jmetal.operator MutationOperator

.. java:import:: org.uma.jmetal.operator SelectionOperator

.. java:import:: org.uma.jmetal.operator.impl.crossover SBXCrossover

.. java:import:: org.uma.jmetal.operator.impl.mutation PolynomialMutation

.. java:import:: org.uma.jmetal.operator.impl.selection BinaryTournamentSelection

.. java:import:: org.uma.jmetal.problem Problem

.. java:import:: org.uma.jmetal.problem.multiobjective.cec2015OptBigDataCompetition BigOpt2015

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.util AbstractAlgorithmRunner

.. java:import:: org.uma.jmetal.util AlgorithmRunner

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: org.uma.jmetal.util JMetalLogger

.. java:import:: org.uma.jmetal.util.comparator RankingAndCrowdingDistanceComparator

.. java:import:: org.uma.jmetal.util.fileoutput SolutionListOutput

.. java:import:: org.uma.jmetal.util.fileoutput.impl DefaultFileOutputContext

.. java:import:: java.lang.reflect InvocationTargetException

.. java:import:: java.util List

NSGAIIBigDataRunner
===================

.. java:package:: org.uma.jmetal.runner.multiobjective
   :noindex:

.. java:type:: public class NSGAIIBigDataRunner extends AbstractAlgorithmRunner

   Class for configuring and running the NSGA-II algorithm to solve a problem of the CEC 2015 Big Optimization competition

   :author: Antonio J. Nebro

Methods
-------
main
^^^^

.. java:method:: public static void main(String[] args) throws JMetalException, ClassNotFoundException, NoSuchMethodException, IllegalAccessException, InvocationTargetException, InstantiationException
   :outertype: NSGAIIBigDataRunner

   :param args: Command line arguments.
   :throws java.io.IOException:
   :throws SecurityException:
   :throws ClassNotFoundException: Invoking command: java org.uma.jmetal.runner.multiobjective.NSGAIIBigDataRunner problemName [referenceFront]

