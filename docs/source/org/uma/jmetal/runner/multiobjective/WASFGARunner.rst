.. java:import:: org.uma.jmetal.algorithm Algorithm

.. java:import:: org.uma.jmetal.algorithm.multiobjective.wasfga WASFGA

.. java:import:: org.uma.jmetal.operator CrossoverOperator

.. java:import:: org.uma.jmetal.operator MutationOperator

.. java:import:: org.uma.jmetal.operator SelectionOperator

.. java:import:: org.uma.jmetal.operator.impl.crossover PMXCrossover

.. java:import:: org.uma.jmetal.operator.impl.mutation PermutationSwapMutation

.. java:import:: org.uma.jmetal.operator.impl.selection BinaryTournamentSelection

.. java:import:: org.uma.jmetal.problem PermutationProblem

.. java:import:: org.uma.jmetal.problem.multiobjective MultiobjectiveTSP

.. java:import:: org.uma.jmetal.solution PermutationSolution

.. java:import:: org.uma.jmetal.util AbstractAlgorithmRunner

.. java:import:: org.uma.jmetal.util AlgorithmRunner

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: org.uma.jmetal.util JMetalLogger

.. java:import:: org.uma.jmetal.util.comparator RankingAndCrowdingDistanceComparator

.. java:import:: org.uma.jmetal.util.evaluator.impl SequentialSolutionListEvaluator

.. java:import:: java.io FileNotFoundException

.. java:import:: java.io IOException

.. java:import:: java.util ArrayList

.. java:import:: java.util List

WASFGARunner
============

.. java:package:: org.uma.jmetal.runner.multiobjective
   :noindex:

.. java:type:: public class WASFGARunner extends AbstractAlgorithmRunner

Methods
-------
main
^^^^

.. java:method:: public static void main(String[] args) throws JMetalException, IOException
   :outertype: WASFGARunner

   :param args: Command line arguments.
   :throws JMetalException:
   :throws FileNotFoundException: Invoking command: java org.uma.jmetal.runner.multiobjective.WASFGABinaryRunner problemName [referenceFront]

