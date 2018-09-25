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

GeneticAlgorithmBuilder
=======================

.. java:package:: org.uma.jmetal.algorithm.singleobjective.geneticalgorithm
   :noindex:

.. java:type:: public class GeneticAlgorithmBuilder<S extends Solution<?>>

   Created by ajnebro on 10/12/14.

Constructors
------------
GeneticAlgorithmBuilder
^^^^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public GeneticAlgorithmBuilder(Problem<S> problem, CrossoverOperator<S> crossoverOperator, MutationOperator<S> mutationOperator)
   :outertype: GeneticAlgorithmBuilder

   Builder constructor

Methods
-------
build
^^^^^

.. java:method:: public Algorithm<S> build()
   :outertype: GeneticAlgorithmBuilder

getCrossoverOperator
^^^^^^^^^^^^^^^^^^^^

.. java:method:: public CrossoverOperator<S> getCrossoverOperator()
   :outertype: GeneticAlgorithmBuilder

getEvaluator
^^^^^^^^^^^^

.. java:method:: public SolutionListEvaluator<S> getEvaluator()
   :outertype: GeneticAlgorithmBuilder

getMaxEvaluations
^^^^^^^^^^^^^^^^^

.. java:method:: public int getMaxEvaluations()
   :outertype: GeneticAlgorithmBuilder

getMutationOperator
^^^^^^^^^^^^^^^^^^^

.. java:method:: public MutationOperator<S> getMutationOperator()
   :outertype: GeneticAlgorithmBuilder

getPopulationSize
^^^^^^^^^^^^^^^^^

.. java:method:: public int getPopulationSize()
   :outertype: GeneticAlgorithmBuilder

getProblem
^^^^^^^^^^

.. java:method:: public Problem<S> getProblem()
   :outertype: GeneticAlgorithmBuilder

getSelectionOperator
^^^^^^^^^^^^^^^^^^^^

.. java:method:: public SelectionOperator<List<S>, S> getSelectionOperator()
   :outertype: GeneticAlgorithmBuilder

getVariant
^^^^^^^^^^

.. java:method:: public GeneticAlgorithmVariant getVariant()
   :outertype: GeneticAlgorithmBuilder

setMaxEvaluations
^^^^^^^^^^^^^^^^^

.. java:method:: public GeneticAlgorithmBuilder<S> setMaxEvaluations(int maxEvaluations)
   :outertype: GeneticAlgorithmBuilder

setPopulationSize
^^^^^^^^^^^^^^^^^

.. java:method:: public GeneticAlgorithmBuilder<S> setPopulationSize(int populationSize)
   :outertype: GeneticAlgorithmBuilder

setSelectionOperator
^^^^^^^^^^^^^^^^^^^^

.. java:method:: public GeneticAlgorithmBuilder<S> setSelectionOperator(SelectionOperator<List<S>, S> selectionOperator)
   :outertype: GeneticAlgorithmBuilder

setSolutionListEvaluator
^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public GeneticAlgorithmBuilder<S> setSolutionListEvaluator(SolutionListEvaluator<S> evaluator)
   :outertype: GeneticAlgorithmBuilder

setVariant
^^^^^^^^^^

.. java:method:: public GeneticAlgorithmBuilder<S> setVariant(GeneticAlgorithmVariant variant)
   :outertype: GeneticAlgorithmBuilder

