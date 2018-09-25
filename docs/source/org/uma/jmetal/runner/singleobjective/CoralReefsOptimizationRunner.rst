.. java:import:: org.uma.jmetal.algorithm Algorithm

.. java:import:: org.uma.jmetal.algorithm.singleobjective.coralreefsoptimization CoralReefsOptimizationBuilder

.. java:import:: org.uma.jmetal.operator CrossoverOperator

.. java:import:: org.uma.jmetal.operator MutationOperator

.. java:import:: org.uma.jmetal.operator SelectionOperator

.. java:import:: org.uma.jmetal.operator.impl.crossover SinglePointCrossover

.. java:import:: org.uma.jmetal.operator.impl.mutation BitFlipMutation

.. java:import:: org.uma.jmetal.operator.impl.selection BinaryTournamentSelection

.. java:import:: org.uma.jmetal.problem BinaryProblem

.. java:import:: org.uma.jmetal.problem.singleobjective OneMax

.. java:import:: org.uma.jmetal.solution BinarySolution

.. java:import:: org.uma.jmetal.util AlgorithmRunner

.. java:import:: org.uma.jmetal.util JMetalLogger

.. java:import:: org.uma.jmetal.util.comparator ObjectiveComparator

.. java:import:: org.uma.jmetal.util.fileoutput SolutionListOutput

.. java:import:: org.uma.jmetal.util.fileoutput.impl DefaultFileOutputContext

.. java:import:: java.util List

CoralReefsOptimizationRunner
============================

.. java:package:: org.uma.jmetal.runner.singleobjective
   :noindex:

.. java:type:: public class CoralReefsOptimizationRunner

   Class to configure and run a coral reefs optimization algorithm. The target problem is OneMax.

   :author: Inacio Medeiros

Methods
-------
main
^^^^

.. java:method:: public static void main(String[] args) throws Exception
   :outertype: CoralReefsOptimizationRunner

   Usage: java org.uma.jmetal.runner.singleobjective.CoralReefsOptimizationRunner

