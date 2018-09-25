.. java:import:: org.uma.jmetal.algorithm Algorithm

.. java:import:: org.uma.jmetal.algorithm.multiobjective.mochc MOCHC45

.. java:import:: org.uma.jmetal.operator CrossoverOperator

.. java:import:: org.uma.jmetal.operator MutationOperator

.. java:import:: org.uma.jmetal.operator SelectionOperator

.. java:import:: org.uma.jmetal.operator.impl.crossover HUXCrossover

.. java:import:: org.uma.jmetal.operator.impl.mutation BitFlipMutation

.. java:import:: org.uma.jmetal.operator.impl.selection RandomSelection

.. java:import:: org.uma.jmetal.operator.impl.selection RankingAndCrowdingSelection

.. java:import:: org.uma.jmetal.problem BinaryProblem

.. java:import:: org.uma.jmetal.solution BinarySolution

.. java:import:: org.uma.jmetal.util AbstractAlgorithmRunner

.. java:import:: org.uma.jmetal.util AlgorithmRunner

.. java:import:: org.uma.jmetal.util JMetalLogger

.. java:import:: org.uma.jmetal.util ProblemUtils

.. java:import:: org.uma.jmetal.util.evaluator.impl SequentialSolutionListEvaluator

.. java:import:: java.util List

MOCHC45Runner
=============

.. java:package:: org.uma.jmetal.runner.multiobjective
   :noindex:

.. java:type:: public class MOCHC45Runner extends AbstractAlgorithmRunner

   This class executes the algorithm described in: A.J. Nebro, E. Alba, G. Molina, F. Chicano, F. Luna, J.J. Durillo "Optimal antenna placement using a new multi-objective chc algorithm". GECCO '07: Proceedings of the 9th annual conference on Genetic and evolutionary computation. London, England. July 2007.

Methods
-------
main
^^^^

.. java:method:: public static void main(String[] args) throws Exception
   :outertype: MOCHC45Runner

