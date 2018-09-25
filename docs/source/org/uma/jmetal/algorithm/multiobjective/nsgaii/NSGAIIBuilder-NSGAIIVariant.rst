.. java:import:: org.uma.jmetal.operator CrossoverOperator

.. java:import:: org.uma.jmetal.operator MutationOperator

.. java:import:: org.uma.jmetal.operator SelectionOperator

.. java:import:: org.uma.jmetal.operator.impl.selection BinaryTournamentSelection

.. java:import:: org.uma.jmetal.problem Problem

.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util AlgorithmBuilder

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: org.uma.jmetal.util.comparator DominanceComparator

.. java:import:: org.uma.jmetal.util.comparator RankingAndCrowdingDistanceComparator

.. java:import:: org.uma.jmetal.util.evaluator SolutionListEvaluator

.. java:import:: org.uma.jmetal.util.evaluator.impl SequentialSolutionListEvaluator

.. java:import:: java.util Comparator

.. java:import:: java.util List

NSGAIIBuilder.NSGAIIVariant
===========================

.. java:package:: org.uma.jmetal.algorithm.multiobjective.nsgaii
   :noindex:

.. java:type:: public enum NSGAIIVariant
   :outertype: NSGAIIBuilder

Enum Constants
--------------
Measures
^^^^^^^^

.. java:field:: public static final NSGAIIBuilder.NSGAIIVariant Measures
   :outertype: NSGAIIBuilder.NSGAIIVariant

NSGAII
^^^^^^

.. java:field:: public static final NSGAIIBuilder.NSGAIIVariant NSGAII
   :outertype: NSGAIIBuilder.NSGAIIVariant

NSGAII45
^^^^^^^^

.. java:field:: public static final NSGAIIBuilder.NSGAIIVariant NSGAII45
   :outertype: NSGAIIBuilder.NSGAIIVariant

SteadyStateNSGAII
^^^^^^^^^^^^^^^^^

.. java:field:: public static final NSGAIIBuilder.NSGAIIVariant SteadyStateNSGAII
   :outertype: NSGAIIBuilder.NSGAIIVariant

