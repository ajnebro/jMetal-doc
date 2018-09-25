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

NSGAIIBuilder
=============

.. java:package:: org.uma.jmetal.algorithm.multiobjective.nsgaii
   :noindex:

.. java:type:: public class NSGAIIBuilder<S extends Solution<?>> implements AlgorithmBuilder<NSGAII<S>>

   :author: Antonio J. Nebro

Constructors
------------
NSGAIIBuilder
^^^^^^^^^^^^^

.. java:constructor:: public NSGAIIBuilder(Problem<S> problem, CrossoverOperator<S> crossoverOperator, MutationOperator<S> mutationOperator)
   :outertype: NSGAIIBuilder

   NSGAIIBuilder constructor

Methods
-------
build
^^^^^

.. java:method:: public NSGAII<S> build()
   :outertype: NSGAIIBuilder

getCrossoverOperator
^^^^^^^^^^^^^^^^^^^^

.. java:method:: public CrossoverOperator<S> getCrossoverOperator()
   :outertype: NSGAIIBuilder

getMaxIterations
^^^^^^^^^^^^^^^^

.. java:method:: public int getMaxIterations()
   :outertype: NSGAIIBuilder

getMutationOperator
^^^^^^^^^^^^^^^^^^^

.. java:method:: public MutationOperator<S> getMutationOperator()
   :outertype: NSGAIIBuilder

getPopulationSize
^^^^^^^^^^^^^^^^^

.. java:method:: public int getPopulationSize()
   :outertype: NSGAIIBuilder

getProblem
^^^^^^^^^^

.. java:method:: public Problem<S> getProblem()
   :outertype: NSGAIIBuilder

getSelectionOperator
^^^^^^^^^^^^^^^^^^^^

.. java:method:: public SelectionOperator<List<S>, S> getSelectionOperator()
   :outertype: NSGAIIBuilder

getSolutionListEvaluator
^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public SolutionListEvaluator<S> getSolutionListEvaluator()
   :outertype: NSGAIIBuilder

setDominanceComparator
^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public NSGAIIBuilder<S> setDominanceComparator(Comparator<S> dominanceComparator)
   :outertype: NSGAIIBuilder

setMaxEvaluations
^^^^^^^^^^^^^^^^^

.. java:method:: public NSGAIIBuilder<S> setMaxEvaluations(int maxEvaluations)
   :outertype: NSGAIIBuilder

setPopulationSize
^^^^^^^^^^^^^^^^^

.. java:method:: public NSGAIIBuilder<S> setPopulationSize(int populationSize)
   :outertype: NSGAIIBuilder

setSelectionOperator
^^^^^^^^^^^^^^^^^^^^

.. java:method:: public NSGAIIBuilder<S> setSelectionOperator(SelectionOperator<List<S>, S> selectionOperator)
   :outertype: NSGAIIBuilder

setSolutionListEvaluator
^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public NSGAIIBuilder<S> setSolutionListEvaluator(SolutionListEvaluator<S> evaluator)
   :outertype: NSGAIIBuilder

setVariant
^^^^^^^^^^

.. java:method:: public NSGAIIBuilder<S> setVariant(NSGAIIVariant variant)
   :outertype: NSGAIIBuilder

