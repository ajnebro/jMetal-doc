.. java:import:: org.knowm.xchart BitmapEncoder.BitmapFormat

.. java:import:: org.uma.jmetal.algorithm Algorithm

.. java:import:: org.uma.jmetal.algorithm.multiobjective.wasfga WASFGAMeasures

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

.. java:import:: org.uma.jmetal.util.comparator RankingAndCrowdingDistanceComparator

.. java:import:: org.uma.jmetal.util.evaluator.impl SequentialSolutionListEvaluator

.. java:import:: java.io IOException

.. java:import:: java.util ArrayList

.. java:import:: java.util List

WASFGAMeasuresRunner3D
======================

.. java:package:: org.uma.jmetal.runner.multiobjective
   :noindex:

.. java:type:: public class WASFGAMeasuresRunner3D extends AbstractAlgorithmRunner

Methods
-------
main
^^^^

.. java:method:: public static void main(String[] args) throws JMetalException, IOException
   :outertype: WASFGAMeasuresRunner3D

   :param args: Command line arguments.
   :throws JMetalException:
   :throws IOException:

