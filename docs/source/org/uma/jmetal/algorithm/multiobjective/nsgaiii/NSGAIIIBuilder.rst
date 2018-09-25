.. java:import:: org.uma.jmetal.operator CrossoverOperator

.. java:import:: org.uma.jmetal.operator MutationOperator

.. java:import:: org.uma.jmetal.operator SelectionOperator

.. java:import:: org.uma.jmetal.problem Problem

.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util AlgorithmBuilder

.. java:import:: org.uma.jmetal.util.evaluator SolutionListEvaluator

.. java:import:: org.uma.jmetal.util.evaluator.impl SequentialSolutionListEvaluator

.. java:import:: java.util List

NSGAIIIBuilder
==============

.. java:package:: org.uma.jmetal.algorithm.multiobjective.nsgaiii
   :noindex:

.. java:type:: public class NSGAIIIBuilder<S extends Solution<?>> implements AlgorithmBuilder<NSGAIII<S>>

   Builder class

Constructors
------------
NSGAIIIBuilder
^^^^^^^^^^^^^^

.. java:constructor:: public NSGAIIIBuilder(Problem<S> problem)
   :outertype: NSGAIIIBuilder

   Builder constructor

Methods
-------
build
^^^^^

.. java:method:: public NSGAIII<S> build()
   :outertype: NSGAIIIBuilder

getCrossoverOperator
^^^^^^^^^^^^^^^^^^^^

.. java:method:: public CrossoverOperator<S> getCrossoverOperator()
   :outertype: NSGAIIIBuilder

getEvaluator
^^^^^^^^^^^^

.. java:method:: public SolutionListEvaluator<S> getEvaluator()
   :outertype: NSGAIIIBuilder

getMaxIterations
^^^^^^^^^^^^^^^^

.. java:method:: public int getMaxIterations()
   :outertype: NSGAIIIBuilder

getMutationOperator
^^^^^^^^^^^^^^^^^^^

.. java:method:: public MutationOperator<S> getMutationOperator()
   :outertype: NSGAIIIBuilder

getPopulationSize
^^^^^^^^^^^^^^^^^

.. java:method:: public int getPopulationSize()
   :outertype: NSGAIIIBuilder

getProblem
^^^^^^^^^^

.. java:method:: public Problem<S> getProblem()
   :outertype: NSGAIIIBuilder

getSelectionOperator
^^^^^^^^^^^^^^^^^^^^

.. java:method:: public SelectionOperator<List<S>, S> getSelectionOperator()
   :outertype: NSGAIIIBuilder

setCrossoverOperator
^^^^^^^^^^^^^^^^^^^^

.. java:method:: public NSGAIIIBuilder<S> setCrossoverOperator(CrossoverOperator<S> crossoverOperator)
   :outertype: NSGAIIIBuilder

setMaxIterations
^^^^^^^^^^^^^^^^

.. java:method:: public NSGAIIIBuilder<S> setMaxIterations(int maxIterations)
   :outertype: NSGAIIIBuilder

setMutationOperator
^^^^^^^^^^^^^^^^^^^

.. java:method:: public NSGAIIIBuilder<S> setMutationOperator(MutationOperator<S> mutationOperator)
   :outertype: NSGAIIIBuilder

setPopulationSize
^^^^^^^^^^^^^^^^^

.. java:method:: public NSGAIIIBuilder<S> setPopulationSize(int populationSize)
   :outertype: NSGAIIIBuilder

setSelectionOperator
^^^^^^^^^^^^^^^^^^^^

.. java:method:: public NSGAIIIBuilder<S> setSelectionOperator(SelectionOperator<List<S>, S> selectionOperator)
   :outertype: NSGAIIIBuilder

setSolutionListEvaluator
^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public NSGAIIIBuilder<S> setSolutionListEvaluator(SolutionListEvaluator<S> evaluator)
   :outertype: NSGAIIIBuilder

