.. java:import:: org.uma.jmetal.algorithm.impl AbstractGeneticAlgorithm

.. java:import:: org.uma.jmetal.operator CrossoverOperator

.. java:import:: org.uma.jmetal.operator MutationOperator

.. java:import:: org.uma.jmetal.operator SelectionOperator

.. java:import:: org.uma.jmetal.problem Problem

.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util.archive BoundedArchive

.. java:import:: org.uma.jmetal.util.comparator DominanceComparator

.. java:import:: org.uma.jmetal.util.comparator RankingAndCrowdingDistanceComparator

.. java:import:: org.uma.jmetal.util.evaluator SolutionListEvaluator

.. java:import:: org.uma.jmetal.util.neighborhood Neighborhood

.. java:import:: org.uma.jmetal.util.solutionattribute Ranking

.. java:import:: org.uma.jmetal.util.solutionattribute.impl CrowdingDistance

.. java:import:: org.uma.jmetal.util.solutionattribute.impl DominanceRanking

.. java:import:: org.uma.jmetal.util.solutionattribute.impl LocationAttribute

.. java:import:: java.util ArrayList

.. java:import:: java.util Collections

.. java:import:: java.util Comparator

.. java:import:: java.util List

MOCell
======

.. java:package:: org.uma.jmetal.algorithm.multiobjective.mocell
   :noindex:

.. java:type:: @SuppressWarnings public class MOCell<S extends Solution<?>> extends AbstractGeneticAlgorithm<S, List<S>>

   :author: JuanJo Durillo
   :param <S>:

Fields
------
archive
^^^^^^^

.. java:field:: protected BoundedArchive<S> archive
   :outertype: MOCell

currentIndividual
^^^^^^^^^^^^^^^^^

.. java:field:: protected int currentIndividual
   :outertype: MOCell

currentNeighbors
^^^^^^^^^^^^^^^^

.. java:field:: protected List<S> currentNeighbors
   :outertype: MOCell

dominanceComparator
^^^^^^^^^^^^^^^^^^^

.. java:field:: protected Comparator<S> dominanceComparator
   :outertype: MOCell

evaluations
^^^^^^^^^^^

.. java:field:: protected int evaluations
   :outertype: MOCell

evaluator
^^^^^^^^^

.. java:field:: protected final SolutionListEvaluator<S> evaluator
   :outertype: MOCell

location
^^^^^^^^

.. java:field:: protected LocationAttribute<S> location
   :outertype: MOCell

maxEvaluations
^^^^^^^^^^^^^^

.. java:field:: protected int maxEvaluations
   :outertype: MOCell

neighborhood
^^^^^^^^^^^^

.. java:field:: protected Neighborhood<S> neighborhood
   :outertype: MOCell

Constructors
------------
MOCell
^^^^^^

.. java:constructor:: public MOCell(Problem<S> problem, int maxEvaluations, int populationSize, BoundedArchive<S> archive, Neighborhood<S> neighborhood, CrossoverOperator<S> crossoverOperator, MutationOperator<S> mutationOperator, SelectionOperator<List<S>, S> selectionOperator, SolutionListEvaluator<S> evaluator)
   :outertype: MOCell

   Constructor

   :param problem:
   :param maxEvaluations:
   :param populationSize:
   :param neighborhood:
   :param crossoverOperator:
   :param mutationOperator:
   :param selectionOperator:
   :param evaluator:

Methods
-------
createInitialPopulation
^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override protected List<S> createInitialPopulation()
   :outertype: MOCell

evaluatePopulation
^^^^^^^^^^^^^^^^^^

.. java:method:: @Override @SuppressWarnings protected List<S> evaluatePopulation(List<S> population)
   :outertype: MOCell

getDescription
^^^^^^^^^^^^^^

.. java:method:: @Override public String getDescription()
   :outertype: MOCell

getName
^^^^^^^

.. java:method:: @Override public String getName()
   :outertype: MOCell

getResult
^^^^^^^^^

.. java:method:: @Override public List<S> getResult()
   :outertype: MOCell

initProgress
^^^^^^^^^^^^

.. java:method:: @Override protected void initProgress()
   :outertype: MOCell

isStoppingConditionReached
^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override protected boolean isStoppingConditionReached()
   :outertype: MOCell

replacement
^^^^^^^^^^^

.. java:method:: @Override protected List<S> replacement(List<S> population, List<S> offspringPopulation)
   :outertype: MOCell

reproduction
^^^^^^^^^^^^

.. java:method:: @Override protected List<S> reproduction(List<S> population)
   :outertype: MOCell

selection
^^^^^^^^^

.. java:method:: @Override protected List<S> selection(List<S> population)
   :outertype: MOCell

updateProgress
^^^^^^^^^^^^^^

.. java:method:: @Override protected void updateProgress()
   :outertype: MOCell

