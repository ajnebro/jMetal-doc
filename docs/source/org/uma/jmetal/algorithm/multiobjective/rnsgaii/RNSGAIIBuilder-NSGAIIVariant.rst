.. java:import:: org.uma.jmetal.operator CrossoverOperator

.. java:import:: org.uma.jmetal.operator MutationOperator

.. java:import:: org.uma.jmetal.operator SelectionOperator

.. java:import:: org.uma.jmetal.operator.impl.selection BinaryTournamentSelection

.. java:import:: org.uma.jmetal.problem Problem

.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util AlgorithmBuilder

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: org.uma.jmetal.util.comparator RankingAndCrowdingDistanceComparator

.. java:import:: org.uma.jmetal.util.evaluator SolutionListEvaluator

.. java:import:: org.uma.jmetal.util.evaluator.impl SequentialSolutionListEvaluator

.. java:import:: java.util List

RNSGAIIBuilder.NSGAIIVariant
============================

.. java:package:: org.uma.jmetal.algorithm.multiobjective.rnsgaii
   :noindex:

.. java:type:: public enum NSGAIIVariant
   :outertype: RNSGAIIBuilder

Enum Constants
--------------
Measures
^^^^^^^^

.. java:field:: public static final RNSGAIIBuilder.NSGAIIVariant Measures
   :outertype: RNSGAIIBuilder.NSGAIIVariant

NSGAII
^^^^^^

.. java:field:: public static final RNSGAIIBuilder.NSGAIIVariant NSGAII
   :outertype: RNSGAIIBuilder.NSGAIIVariant

NSGAII45
^^^^^^^^

.. java:field:: public static final RNSGAIIBuilder.NSGAIIVariant NSGAII45
   :outertype: RNSGAIIBuilder.NSGAIIVariant

SteadyStateNSGAII
^^^^^^^^^^^^^^^^^

.. java:field:: public static final RNSGAIIBuilder.NSGAIIVariant SteadyStateNSGAII
   :outertype: RNSGAIIBuilder.NSGAIIVariant

