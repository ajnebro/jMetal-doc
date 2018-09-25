.. java:import:: org.uma.jmetal.algorithm Algorithm

.. java:import:: org.uma.jmetal.operator CrossoverOperator

.. java:import:: org.uma.jmetal.operator MutationOperator

.. java:import:: org.uma.jmetal.operator SelectionOperator

.. java:import:: org.uma.jmetal.operator.impl.selection BinaryTournamentSelection

.. java:import:: org.uma.jmetal.problem Problem

.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: org.uma.jmetal.util.evaluator SolutionListEvaluator

.. java:import:: org.uma.jmetal.util.evaluator.impl SequentialSolutionListEvaluator

.. java:import:: java.util List

GeneticAlgorithmBuilder.GeneticAlgorithmVariant
===============================================

.. java:package:: org.uma.jmetal.algorithm.singleobjective.geneticalgorithm
   :noindex:

.. java:type:: public enum GeneticAlgorithmVariant
   :outertype: GeneticAlgorithmBuilder

Enum Constants
--------------
GENERATIONAL
^^^^^^^^^^^^

.. java:field:: public static final GeneticAlgorithmBuilder.GeneticAlgorithmVariant GENERATIONAL
   :outertype: GeneticAlgorithmBuilder.GeneticAlgorithmVariant

STEADY_STATE
^^^^^^^^^^^^

.. java:field:: public static final GeneticAlgorithmBuilder.GeneticAlgorithmVariant STEADY_STATE
   :outertype: GeneticAlgorithmBuilder.GeneticAlgorithmVariant

