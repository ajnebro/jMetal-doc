.. java:import:: org.uma.jmetal.algorithm Algorithm

.. java:import:: org.uma.jmetal.algorithm.multiobjective.gde3 GDE3

.. java:import:: org.uma.jmetal.algorithm.multiobjective.gde3 GDE3Builder

.. java:import:: org.uma.jmetal.operator.impl.crossover DifferentialEvolutionCrossover

.. java:import:: org.uma.jmetal.operator.impl.selection DifferentialEvolutionSelection

.. java:import:: org.uma.jmetal.problem DoubleProblem

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.util AbstractAlgorithmRunner

.. java:import:: org.uma.jmetal.util AlgorithmRunner

.. java:import:: org.uma.jmetal.util JMetalLogger

.. java:import:: org.uma.jmetal.util ProblemUtils

.. java:import:: org.uma.jmetal.util.evaluator SolutionListEvaluator

.. java:import:: org.uma.jmetal.util.evaluator.impl MultithreadedSolutionListEvaluator

.. java:import:: java.io FileNotFoundException

.. java:import:: java.util List

ParallelGDE3Runner
==================

.. java:package:: org.uma.jmetal.runner.multiobjective
   :noindex:

.. java:type:: public class ParallelGDE3Runner extends AbstractAlgorithmRunner

   Class for configuring and running the GDE3 algorithm (parallel version)

   :author: Antonio J. Nebro

Methods
-------
main
^^^^

.. java:method:: public static void main(String[] args) throws FileNotFoundException
   :outertype: ParallelGDE3Runner

   :param args: Command line arguments.
   :throws SecurityException: Invoking command: java org.uma.jmetal.runner.multiobjective.ParallelGDE3Runner problemName [referenceFront]

