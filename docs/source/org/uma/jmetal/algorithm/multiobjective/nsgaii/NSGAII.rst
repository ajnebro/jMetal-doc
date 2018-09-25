.. java:import:: org.uma.jmetal.algorithm.impl AbstractGeneticAlgorithm

.. java:import:: org.uma.jmetal.operator CrossoverOperator

.. java:import:: org.uma.jmetal.operator MutationOperator

.. java:import:: org.uma.jmetal.operator SelectionOperator

.. java:import:: org.uma.jmetal.operator.impl.selection RankingAndCrowdingSelection

.. java:import:: org.uma.jmetal.problem Problem

.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util SolutionListUtils

.. java:import:: org.uma.jmetal.util.comparator DominanceComparator

.. java:import:: org.uma.jmetal.util.evaluator SolutionListEvaluator

.. java:import:: java.util ArrayList

.. java:import:: java.util Comparator

.. java:import:: java.util List

NSGAII
======

.. java:package:: org.uma.jmetal.algorithm.multiobjective.nsgaii
   :noindex:

.. java:type:: @SuppressWarnings public class NSGAII<S extends Solution<?>> extends AbstractGeneticAlgorithm<S, List<S>>

   :author: Antonio J. Nebro

Fields
------
dominanceComparator
^^^^^^^^^^^^^^^^^^^

.. java:field:: protected Comparator<S> dominanceComparator
   :outertype: NSGAII

evaluations
^^^^^^^^^^^

.. java:field:: protected int evaluations
   :outertype: NSGAII

evaluator
^^^^^^^^^

.. java:field:: protected final SolutionListEvaluator<S> evaluator
   :outertype: NSGAII

maxEvaluations
^^^^^^^^^^^^^^

.. java:field:: protected final int maxEvaluations
   :outertype: NSGAII

Constructors
------------
NSGAII
^^^^^^

.. java:constructor:: public NSGAII(Problem<S> problem, int maxEvaluations, int populationSize, CrossoverOperator<S> crossoverOperator, MutationOperator<S> mutationOperator, SelectionOperator<List<S>, S> selectionOperator, SolutionListEvaluator<S> evaluator)
   :outertype: NSGAII

   Constructor

NSGAII
^^^^^^

.. java:constructor:: public NSGAII(Problem<S> problem, int maxEvaluations, int populationSize, CrossoverOperator<S> crossoverOperator, MutationOperator<S> mutationOperator, SelectionOperator<List<S>, S> selectionOperator, Comparator<S> dominanceComparator, SolutionListEvaluator<S> evaluator)
   :outertype: NSGAII

   Constructor

Methods
-------
evaluatePopulation
^^^^^^^^^^^^^^^^^^

.. java:method:: @Override protected List<S> evaluatePopulation(List<S> population)
   :outertype: NSGAII

getDescription
^^^^^^^^^^^^^^

.. java:method:: @Override public String getDescription()
   :outertype: NSGAII

getName
^^^^^^^

.. java:method:: @Override public String getName()
   :outertype: NSGAII

getNonDominatedSolutions
^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: protected List<S> getNonDominatedSolutions(List<S> solutionList)
   :outertype: NSGAII

getResult
^^^^^^^^^

.. java:method:: @Override public List<S> getResult()
   :outertype: NSGAII

initProgress
^^^^^^^^^^^^

.. java:method:: @Override protected void initProgress()
   :outertype: NSGAII

isStoppingConditionReached
^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override protected boolean isStoppingConditionReached()
   :outertype: NSGAII

replacement
^^^^^^^^^^^

.. java:method:: @Override protected List<S> replacement(List<S> population, List<S> offspringPopulation)
   :outertype: NSGAII

updateProgress
^^^^^^^^^^^^^^

.. java:method:: @Override protected void updateProgress()
   :outertype: NSGAII

