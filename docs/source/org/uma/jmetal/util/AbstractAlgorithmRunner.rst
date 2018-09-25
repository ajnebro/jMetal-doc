.. java:import:: org.uma.jmetal.qualityindicator.impl.hypervolume PISAHypervolume

.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util.fileoutput SolutionListOutput

.. java:import:: org.uma.jmetal.util.fileoutput.impl DefaultFileOutputContext

.. java:import:: org.uma.jmetal.util.front Front

.. java:import:: org.uma.jmetal.util.front.imp ArrayFront

.. java:import:: org.uma.jmetal.util.front.util FrontNormalizer

.. java:import:: org.uma.jmetal.util.front.util FrontUtils

.. java:import:: org.uma.jmetal.util.point PointSolution

.. java:import:: org.uma.jmetal.util.pseudorandom JMetalRandom

.. java:import:: java.io FileNotFoundException

.. java:import:: java.util List

AbstractAlgorithmRunner
=======================

.. java:package:: org.uma.jmetal.util
   :noindex:

.. java:type:: public abstract class AbstractAlgorithmRunner

   Abstract class for Runner classes

   :author: Antonio J. Nebro

Methods
-------
printFinalSolutionSet
^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public static void printFinalSolutionSet(List<? extends Solution<?>> population)
   :outertype: AbstractAlgorithmRunner

   Write the population into two files and prints some data on screen

   :param population:

printQualityIndicators
^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public static <S extends Solution<?>> void printQualityIndicators(List<S> population, String paretoFrontFile) throws FileNotFoundException
   :outertype: AbstractAlgorithmRunner

   Print all the available quality indicators

   :param population:
   :param paretoFrontFile:
   :throws FileNotFoundException:

