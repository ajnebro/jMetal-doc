.. java:import:: org.uma.jmetal.algorithm Algorithm

.. java:import:: org.uma.jmetal.algorithm.multiobjective.nsgaii NSGAII45

.. java:import:: org.uma.jmetal.operator CrossoverOperator

.. java:import:: org.uma.jmetal.operator MutationOperator

.. java:import:: org.uma.jmetal.operator SelectionOperator

.. java:import:: org.uma.jmetal.operator.impl.crossover SBXCrossover

.. java:import:: org.uma.jmetal.operator.impl.mutation PolynomialMutation

.. java:import:: org.uma.jmetal.operator.impl.selection BinaryTournamentSelection

.. java:import:: org.uma.jmetal.problem Problem

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.util.comparator RankingAndCrowdingDistanceComparator

.. java:import:: org.uma.jmetal.util.evaluator.impl SequentialSolutionListEvaluator

.. java:import:: java.io FileNotFoundException

.. java:import:: java.util List

NSGAII45Runner
==============

.. java:package:: org.uma.jmetal.runner.multiobjective
   :noindex:

.. java:type:: public class NSGAII45Runner extends AbstractAlgorithmRunner

   Class to configure and run the implementation of the NSGA-II algorithm included in \ :java:ref:`NSGAII45`\

   :author: Antonio J. Nebro

Methods
-------
main
^^^^

.. java:method:: public static void main(String[] args) throws JMetalException, FileNotFoundException
   :outertype: NSGAII45Runner

   :param args: Command line arguments.
   :throws JMetalException:
   :throws FileNotFoundException: Invoking command: java org.uma.jmetal.runner.multiobjective.NSGAII45Runner problemName [referenceFront]

