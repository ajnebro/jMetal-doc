.. java:import:: org.uma.jmetal.qualityindicator QualityIndicator

.. java:import:: org.uma.jmetal.qualityindicator.impl.hypervolume PISAHypervolume

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: org.uma.jmetal.util JMetalLogger

.. java:import:: org.uma.jmetal.util.front Front

.. java:import:: org.uma.jmetal.util.front.imp ArrayFront

.. java:import:: org.uma.jmetal.util.front.util FrontNormalizer

.. java:import:: org.uma.jmetal.util.front.util FrontUtils

.. java:import:: org.uma.jmetal.util.point PointSolution

.. java:import:: java.io FileNotFoundException

.. java:import:: java.util ArrayList

.. java:import:: java.util List

CommandLineIndicatorRunner
==========================

.. java:package:: org.uma.jmetal.qualityIndicator
   :noindex:

.. java:type:: public class CommandLineIndicatorRunner

   Class for executing quality indicators from the command line. An optional argument allows to indicate whether the fronts are to be normalized by the quality indicators. Invoking command: mvn -pl jmetal-exec exec:java -Dexec.mainClass="org.uma.jmetal.qualityIndicator.CommandLineIndicatorRunner" -Dexec.args="indicator referenceFront front normalize"

   :author: Antonio J. Nebro

Methods
-------
main
^^^^

.. java:method:: public static void main(String[] args) throws Exception
   :outertype: CommandLineIndicatorRunner

