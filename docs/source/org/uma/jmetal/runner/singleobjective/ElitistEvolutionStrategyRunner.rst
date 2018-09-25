.. java:import:: org.uma.jmetal.algorithm Algorithm

.. java:import:: org.uma.jmetal.algorithm.singleobjective.evolutionstrategy EvolutionStrategyBuilder

.. java:import:: org.uma.jmetal.operator MutationOperator

.. java:import:: org.uma.jmetal.operator.impl.mutation BitFlipMutation

.. java:import:: org.uma.jmetal.problem BinaryProblem

.. java:import:: org.uma.jmetal.problem.singleobjective OneMax

.. java:import:: org.uma.jmetal.solution BinarySolution

.. java:import:: org.uma.jmetal.util AlgorithmRunner

.. java:import:: org.uma.jmetal.util JMetalLogger

.. java:import:: org.uma.jmetal.util.fileoutput SolutionListOutput

.. java:import:: org.uma.jmetal.util.fileoutput.impl DefaultFileOutputContext

.. java:import:: java.util ArrayList

.. java:import:: java.util List

ElitistEvolutionStrategyRunner
==============================

.. java:package:: org.uma.jmetal.runner.singleobjective
   :noindex:

.. java:type:: public class ElitistEvolutionStrategyRunner

   Class to configure and run an elitist (mu + lambda) evolution strategy. The target problem is OneMax.

   :author: Antonio J. Nebro

Methods
-------
main
^^^^

.. java:method:: public static void main(String[] args) throws Exception
   :outertype: ElitistEvolutionStrategyRunner

   Usage: java org.uma.jmetal.runner.singleobjective.ElitistEvolutionStrategyRunner

