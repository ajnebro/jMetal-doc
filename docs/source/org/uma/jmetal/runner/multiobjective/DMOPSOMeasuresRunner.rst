.. java:import:: org.knowm.xchart BitmapEncoder.BitmapFormat

.. java:import:: org.uma.jmetal.algorithm.multiobjective.dmopso DMOPSO.FunctionType

.. java:import:: org.uma.jmetal.algorithm.multiobjective.dmopso DMOPSOMeasures

.. java:import:: org.uma.jmetal.measure MeasureListener

.. java:import:: org.uma.jmetal.measure MeasureManager

.. java:import:: org.uma.jmetal.measure.impl BasicMeasure

.. java:import:: org.uma.jmetal.measure.impl CountingMeasure

.. java:import:: org.uma.jmetal.problem DoubleProblem

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.util AbstractAlgorithmRunner

.. java:import:: org.uma.jmetal.util AlgorithmRunner

.. java:import:: org.uma.jmetal.util JMetalLogger

.. java:import:: org.uma.jmetal.util ProblemUtils

.. java:import:: org.uma.jmetal.util.chartcontainer ChartContainer

.. java:import:: org.uma.jmetal.util.front.imp ArrayFront

.. java:import:: java.util List

DMOPSOMeasuresRunner
====================

.. java:package:: org.uma.jmetal.runner.multiobjective
   :noindex:

.. java:type:: public class DMOPSOMeasuresRunner extends AbstractAlgorithmRunner

   Class for configuring and running the DMOPSO algorithm

   :author: Antonio J. Nebro

Methods
-------
main
^^^^

.. java:method:: public static void main(String[] args) throws Exception
   :outertype: DMOPSOMeasuresRunner

   :param args: Command line arguments.
   :throws SecurityException: Invoking command: java org.uma.jmetal.runner.multiobjective.DMOPSORunner problemName [referenceFront]

