.. java:import:: org.uma.jmetal.algorithm Algorithm

.. java:import:: org.uma.jmetal.algorithm.multiobjective.mocell MOCellBuilder

.. java:import:: org.uma.jmetal.operator CrossoverOperator

.. java:import:: org.uma.jmetal.operator MutationOperator

.. java:import:: org.uma.jmetal.operator SelectionOperator

.. java:import:: org.uma.jmetal.operator.impl.crossover SBXCrossover

.. java:import:: org.uma.jmetal.operator.impl.mutation PolynomialMutation

.. java:import:: org.uma.jmetal.operator.impl.selection BinaryTournamentSelection

.. java:import:: org.uma.jmetal.problem Problem

.. java:import:: org.uma.jmetal.problem.multiobjective.dtlz DTLZ1

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.util.archive.impl CrowdingDistanceArchive

.. java:import:: org.uma.jmetal.util.comparator RankingAndCrowdingDistanceComparator

.. java:import:: java.io FileNotFoundException

.. java:import:: java.util List

MOCellRunner
============

.. java:package:: org.uma.jmetal.runner.multiobjective
   :noindex:

.. java:type:: public class MOCellRunner extends AbstractAlgorithmRunner

   Class to configure and run the MOCell algorithm

   :author: Antonio J. Nebro

Methods
-------
main
^^^^

.. java:method:: public static void main(String[] args) throws JMetalException, FileNotFoundException
   :outertype: MOCellRunner

   :param args: Command line arguments.
   :throws JMetalException:
   :throws FileNotFoundException: Invoking command: java org.uma.jmetal.runner.multiobjective.MOCellRunner problemName [referenceFront]

