.. java:import:: org.uma.jmetal.algorithm Algorithm

.. java:import:: org.uma.jmetal.algorithm.multiobjective.cellde CellDE45

.. java:import:: org.uma.jmetal.operator SelectionOperator

.. java:import:: org.uma.jmetal.operator.impl.crossover DifferentialEvolutionCrossover

.. java:import:: org.uma.jmetal.operator.impl.selection BinaryTournamentSelection

.. java:import:: org.uma.jmetal.problem Problem

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.util.archive.impl CrowdingDistanceArchive

.. java:import:: org.uma.jmetal.util.comparator RankingAndCrowdingDistanceComparator

.. java:import:: org.uma.jmetal.util.evaluator.impl SequentialSolutionListEvaluator

.. java:import:: org.uma.jmetal.util.neighborhood.impl C9

.. java:import:: java.io FileNotFoundException

.. java:import:: java.util List

CellDERunner
============

.. java:package:: org.uma.jmetal.runner.multiobjective
   :noindex:

.. java:type:: public class CellDERunner extends AbstractAlgorithmRunner

   Class to configure and run the MOCell algorithm

   :author: Antonio J. Nebro

Methods
-------
main
^^^^

.. java:method:: public static void main(String[] args) throws JMetalException, FileNotFoundException
   :outertype: CellDERunner

   :param args: Command line arguments.
   :throws JMetalException:
   :throws FileNotFoundException: Invoking command: java org.uma.jmetal.runner.multiobjective.MOCellRunner problemName [referenceFront]

