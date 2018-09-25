.. java:import:: org.uma.jmetal.algorithm Algorithm

.. java:import:: org.uma.jmetal.algorithm.impl AbstractGeneticAlgorithm

.. java:import:: org.uma.jmetal.operator CrossoverOperator

.. java:import:: org.uma.jmetal.operator MutationOperator

.. java:import:: org.uma.jmetal.operator SelectionOperator

.. java:import:: org.uma.jmetal.problem Problem

.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util SolutionListUtils

.. java:import:: org.uma.jmetal.util.comparator CrowdingDistanceComparator

.. java:import:: org.uma.jmetal.util.evaluator SolutionListEvaluator

.. java:import:: org.uma.jmetal.util.solutionattribute Ranking

.. java:import:: org.uma.jmetal.util.solutionattribute.impl CrowdingDistance

.. java:import:: org.uma.jmetal.util.solutionattribute.impl DominanceRanking

.. java:import:: java.util ArrayList

.. java:import:: java.util Collections

.. java:import:: java.util List

NSGAII45
========

.. java:package:: org.uma.jmetal.algorithm.multiobjective.nsgaii
   :noindex:

.. java:type:: @SuppressWarnings public class NSGAII45<S extends Solution<?>> implements Algorithm<List<S>>

   Implementation of NSGA-II following the scheme used in jMetal4.5 and former versions, i.e, without implementing the \ :java:ref:`AbstractGeneticAlgorithm`\  interface.

   :author: Antonio J. Nebro

Fields
------
crossoverOperator
^^^^^^^^^^^^^^^^^

.. java:field:: protected CrossoverOperator<S> crossoverOperator
   :outertype: NSGAII45

evaluations
^^^^^^^^^^^

.. java:field:: protected int evaluations
   :outertype: NSGAII45

evaluator
^^^^^^^^^

.. java:field:: protected final SolutionListEvaluator<S> evaluator
   :outertype: NSGAII45

maxEvaluations
^^^^^^^^^^^^^^

.. java:field:: protected final int maxEvaluations
   :outertype: NSGAII45

mutationOperator
^^^^^^^^^^^^^^^^

.. java:field:: protected MutationOperator<S> mutationOperator
   :outertype: NSGAII45

population
^^^^^^^^^^

.. java:field:: protected List<S> population
   :outertype: NSGAII45

populationSize
^^^^^^^^^^^^^^

.. java:field:: protected final int populationSize
   :outertype: NSGAII45

problem
^^^^^^^

.. java:field:: protected final Problem<S> problem
   :outertype: NSGAII45

selectionOperator
^^^^^^^^^^^^^^^^^

.. java:field:: protected SelectionOperator<List<S>, S> selectionOperator
   :outertype: NSGAII45

Constructors
------------
NSGAII45
^^^^^^^^

.. java:constructor:: public NSGAII45(Problem<S> problem, int maxEvaluations, int populationSize, CrossoverOperator<S> crossoverOperator, MutationOperator<S> mutationOperator, SelectionOperator<List<S>, S> selectionOperator, SolutionListEvaluator<S> evaluator)
   :outertype: NSGAII45

   Constructor

Methods
-------
addLastRankedSolutionsToPopulation
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: protected void addLastRankedSolutionsToPopulation(Ranking<S> ranking, int rank, List<S> population)
   :outertype: NSGAII45

addRankedSolutionsToPopulation
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: protected void addRankedSolutionsToPopulation(Ranking<S> ranking, int rank, List<S> population)
   :outertype: NSGAII45

computeRanking
^^^^^^^^^^^^^^

.. java:method:: protected Ranking<S> computeRanking(List<S> solutionList)
   :outertype: NSGAII45

createInitialPopulation
^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: protected List<S> createInitialPopulation()
   :outertype: NSGAII45

crowdingDistanceSelection
^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: protected List<S> crowdingDistanceSelection(Ranking<S> ranking)
   :outertype: NSGAII45

evaluatePopulation
^^^^^^^^^^^^^^^^^^

.. java:method:: protected List<S> evaluatePopulation(List<S> population)
   :outertype: NSGAII45

getDescription
^^^^^^^^^^^^^^

.. java:method:: @Override public String getDescription()
   :outertype: NSGAII45

getName
^^^^^^^

.. java:method:: @Override public String getName()
   :outertype: NSGAII45

getNonDominatedSolutions
^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: protected List<S> getNonDominatedSolutions(List<S> solutionList)
   :outertype: NSGAII45

getResult
^^^^^^^^^

.. java:method:: @Override public List<S> getResult()
   :outertype: NSGAII45

populationIsNotFull
^^^^^^^^^^^^^^^^^^^

.. java:method:: protected boolean populationIsNotFull(List<S> population)
   :outertype: NSGAII45

run
^^^

.. java:method:: @Override public void run()
   :outertype: NSGAII45

   Run method

subfrontFillsIntoThePopulation
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: protected boolean subfrontFillsIntoThePopulation(Ranking<S> ranking, int rank, List<S> population)
   :outertype: NSGAII45

