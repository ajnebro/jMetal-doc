.. java:import:: org.uma.jmetal.algorithm Algorithm

.. java:import:: org.uma.jmetal.algorithm.multiobjective.pesa2 PESA2Builder

.. java:import:: org.uma.jmetal.operator CrossoverOperator

.. java:import:: org.uma.jmetal.operator MutationOperator

.. java:import:: org.uma.jmetal.operator.impl.crossover SBXCrossover

.. java:import:: org.uma.jmetal.operator.impl.mutation PolynomialMutation

.. java:import:: org.uma.jmetal.problem Problem

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.util.evaluator SolutionListEvaluator

.. java:import:: org.uma.jmetal.util.evaluator.impl MultithreadedSolutionListEvaluator

.. java:import:: java.io FileNotFoundException

.. java:import:: java.util List

ParallelPESA2Runner
===================

.. java:package:: org.uma.jmetal.runner.multiobjective
   :noindex:

.. java:type:: public class ParallelPESA2Runner extends AbstractAlgorithmRunner

   Class for configuring and running the PESA2 algorithm (parallel version)

   :author: Antonio J. Nebro

Methods
-------
main
^^^^

.. java:method:: public static void main(String[] args) throws JMetalException, FileNotFoundException
   :outertype: ParallelPESA2Runner

   :param args: Command line arguments.
   :throws SecurityException: Invoking command: java org.uma.jmetal.runner.multiobjective.ParallelPESA2Runner problemName [referenceFront]

