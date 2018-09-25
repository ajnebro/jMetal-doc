.. java:import:: org.knowm.xchart BitmapEncoder

.. java:import:: org.uma.jmetal.algorithm Algorithm

.. java:import:: org.uma.jmetal.algorithm.multiobjective.smpso SMPSOBuilder

.. java:import:: org.uma.jmetal.algorithm.multiobjective.smpso SMPSOMeasures

.. java:import:: org.uma.jmetal.measure MeasureListener

.. java:import:: org.uma.jmetal.measure MeasureManager

.. java:import:: org.uma.jmetal.measure.impl BasicMeasure

.. java:import:: org.uma.jmetal.measure.impl CountingMeasure

.. java:import:: org.uma.jmetal.operator MutationOperator

.. java:import:: org.uma.jmetal.operator.impl.mutation PolynomialMutation

.. java:import:: org.uma.jmetal.problem DoubleProblem

.. java:import:: org.uma.jmetal.problem.multiobjective.dtlz DTLZ1

.. java:import:: org.uma.jmetal.problem.multiobjective.dtlz DTLZ3

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.util.archive BoundedArchive

.. java:import:: org.uma.jmetal.util.archive.impl CrowdingDistanceArchive

.. java:import:: org.uma.jmetal.util.chartcontainer ChartContainer

.. java:import:: org.uma.jmetal.util.evaluator.impl SequentialSolutionListEvaluator

.. java:import:: org.uma.jmetal.util.pseudorandom.impl MersenneTwisterGenerator

.. java:import:: java.io IOException

.. java:import:: java.util List

SMPSOMeasuresWithChartsRunner
=============================

.. java:package:: org.uma.jmetal.runner.multiobjective
   :noindex:

.. java:type:: public class SMPSOMeasuresWithChartsRunner extends AbstractAlgorithmRunner

   Class to configure and run the NSGA-II algorithm (variant with measures)

Methods
-------
main
^^^^

.. java:method:: public static void main(String[] args) throws JMetalException, InterruptedException, IOException
   :outertype: SMPSOMeasuresWithChartsRunner

   :param args: Command line arguments.
   :throws SecurityException: Invoking command: java org.uma.jmetal.runner.multiobjective.NSGAIIMeasuresRunner problemName [referenceFront]

