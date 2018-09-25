.. java:import:: org.knowm.xchart BitmapEncoder.BitmapFormat

.. java:import:: org.uma.jmetal.algorithm Algorithm

.. java:import:: org.uma.jmetal.algorithm.multiobjective.nsgaii NSGAIIBuilder

.. java:import:: org.uma.jmetal.algorithm.multiobjective.nsgaii NSGAIIMeasures

.. java:import:: org.uma.jmetal.measure MeasureListener

.. java:import:: org.uma.jmetal.measure MeasureManager

.. java:import:: org.uma.jmetal.measure.impl BasicMeasure

.. java:import:: org.uma.jmetal.measure.impl CountingMeasure

.. java:import:: org.uma.jmetal.operator CrossoverOperator

.. java:import:: org.uma.jmetal.operator MutationOperator

.. java:import:: org.uma.jmetal.operator SelectionOperator

.. java:import:: org.uma.jmetal.operator.impl.crossover SBXCrossover

.. java:import:: org.uma.jmetal.operator.impl.mutation PolynomialMutation

.. java:import:: org.uma.jmetal.operator.impl.selection BinaryTournamentSelection

.. java:import:: org.uma.jmetal.problem Problem

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.util.chartcontainer ChartContainer

.. java:import:: org.uma.jmetal.util.comparator GDominanceComparator

.. java:import:: org.uma.jmetal.util.comparator RankingAndCrowdingDistanceComparator

.. java:import:: org.uma.jmetal.util.front.imp ArrayFront

.. java:import:: java.io IOException

.. java:import:: java.util Arrays

.. java:import:: java.util List

GNSGAIIMeasuresWithChartsRunner
===============================

.. java:package:: org.uma.jmetal.runner.multiobjective
   :noindex:

.. java:type:: public class GNSGAIIMeasuresWithChartsRunner extends AbstractAlgorithmRunner

   Class to configure and run the NSGA-II algorithm (variant with measures) with the G-Dominance Comparator.

Methods
-------
main
^^^^

.. java:method:: public static void main(String[] args) throws JMetalException, InterruptedException, IOException
   :outertype: GNSGAIIMeasuresWithChartsRunner

   :param args: Command line arguments.
   :throws SecurityException: Invoking command: java org.uma.jmetal.runner.multiobjective.NSGAIIMeasuresRunner problemName [referenceFront]

