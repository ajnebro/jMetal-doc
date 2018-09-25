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

RNSGAIIBuilder
==============

.. java:package:: org.uma.jmetal.algorithm.multiobjective.rnsgaii
   :noindex:

.. java:type:: public class RNSGAIIBuilder<S extends Solution<?>> implements AlgorithmBuilder<RNSGAII<S>>

   :author: Antonio J. Nebro

Constructors
------------
RNSGAIIBuilder
^^^^^^^^^^^^^^

.. java:constructor:: public RNSGAIIBuilder(Problem<S> problem, CrossoverOperator<S> crossoverOperator, MutationOperator<S> mutationOperator, List<Double> interestPoint, double epsilon)
   :outertype: RNSGAIIBuilder

   NSGAIIBuilder constructor

Methods
-------
build
^^^^^

.. java:method:: public RNSGAII<S> build()
   :outertype: RNSGAIIBuilder

getCrossoverOperator
^^^^^^^^^^^^^^^^^^^^

.. java:method:: public CrossoverOperator<S> getCrossoverOperator()
   :outertype: RNSGAIIBuilder

getMaxIterations
^^^^^^^^^^^^^^^^

.. java:method:: public int getMaxIterations()
   :outertype: RNSGAIIBuilder

getMutationOperator
^^^^^^^^^^^^^^^^^^^

.. java:method:: public MutationOperator<S> getMutationOperator()
   :outertype: RNSGAIIBuilder

getPopulationSize
^^^^^^^^^^^^^^^^^

.. java:method:: public int getPopulationSize()
   :outertype: RNSGAIIBuilder

getProblem
^^^^^^^^^^

.. java:method:: public Problem<S> getProblem()
   :outertype: RNSGAIIBuilder

getSelectionOperator
^^^^^^^^^^^^^^^^^^^^

.. java:method:: public SelectionOperator<List<S>, S> getSelectionOperator()
   :outertype: RNSGAIIBuilder

getSolutionListEvaluator
^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public SolutionListEvaluator<S> getSolutionListEvaluator()
   :outertype: RNSGAIIBuilder

setMaxEvaluations
^^^^^^^^^^^^^^^^^

.. java:method:: public RNSGAIIBuilder<S> setMaxEvaluations(int maxEvaluations)
   :outertype: RNSGAIIBuilder

setPopulationSize
^^^^^^^^^^^^^^^^^

.. java:method:: public RNSGAIIBuilder<S> setPopulationSize(int populationSize)
   :outertype: RNSGAIIBuilder

setSelectionOperator
^^^^^^^^^^^^^^^^^^^^

.. java:method:: public RNSGAIIBuilder<S> setSelectionOperator(SelectionOperator<List<S>, S> selectionOperator)
   :outertype: RNSGAIIBuilder

setSolutionListEvaluator
^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public RNSGAIIBuilder<S> setSolutionListEvaluator(SolutionListEvaluator<S> evaluator)
   :outertype: RNSGAIIBuilder

setVariant
^^^^^^^^^^

.. java:method:: public RNSGAIIBuilder<S> setVariant(NSGAIIVariant variant)
   :outertype: RNSGAIIBuilder

