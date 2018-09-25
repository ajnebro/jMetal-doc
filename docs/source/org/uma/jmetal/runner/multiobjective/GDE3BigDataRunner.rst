.. java:import:: org.uma.jmetal.algorithm Algorithm

.. java:import:: org.uma.jmetal.algorithm.multiobjective.gde3 GDE3

.. java:import:: org.uma.jmetal.algorithm.multiobjective.gde3 GDE3Builder

.. java:import:: org.uma.jmetal.operator.impl.crossover DifferentialEvolutionCrossover

.. java:import:: org.uma.jmetal.operator.impl.selection DifferentialEvolutionSelection

.. java:import:: org.uma.jmetal.problem DoubleProblem

.. java:import:: org.uma.jmetal.problem.multiobjective.cec2015OptBigDataCompetition BigOpt2015

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.util AlgorithmRunner

.. java:import:: org.uma.jmetal.util JMetalLogger

.. java:import:: org.uma.jmetal.util.fileoutput SolutionListOutput

.. java:import:: org.uma.jmetal.util.fileoutput.impl DefaultFileOutputContext

.. java:import:: java.util List

GDE3BigDataRunner
=================

.. java:package:: org.uma.jmetal.runner.multiobjective
   :noindex:

.. java:type:: public class GDE3BigDataRunner

   Class for configuring and running the GDE3 algorithm for solving a problem of the Big Optimization competition at CEC2015

   :author: Antonio J. Nebro

Methods
-------
main
^^^^

.. java:method:: public static void main(String[] args)
   :outertype: GDE3BigDataRunner

   :param args: Command line arguments.
   :throws SecurityException: Invoking command: mvn -pl jmetal-exec exec:java -Dexec.mainClass="org.uma.jmetal.runner.multiobjective.GDE3BigDataRunner" -Dexec.args="[problemName]"

