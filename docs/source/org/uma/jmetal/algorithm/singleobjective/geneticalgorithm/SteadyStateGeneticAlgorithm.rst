.. java:import:: org.uma.jmetal.algorithm.impl AbstractGeneticAlgorithm

.. java:import:: org.uma.jmetal.operator CrossoverOperator

.. java:import:: org.uma.jmetal.operator MutationOperator

.. java:import:: org.uma.jmetal.operator SelectionOperator

.. java:import:: org.uma.jmetal.problem Problem

.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util.comparator ObjectiveComparator

.. java:import:: java.util ArrayList

.. java:import:: java.util Collections

.. java:import:: java.util Comparator

.. java:import:: java.util List

SteadyStateGeneticAlgorithm
===========================

.. java:package:: org.uma.jmetal.algorithm.singleobjective.geneticalgorithm
   :noindex:

.. java:type:: @SuppressWarnings public class SteadyStateGeneticAlgorithm<S extends Solution<?>> extends AbstractGeneticAlgorithm<S, S>

   :author: Antonio J. Nebro

Constructors
------------
SteadyStateGeneticAlgorithm
^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public SteadyStateGeneticAlgorithm(Problem<S> problem, int maxEvaluations, int populationSize, CrossoverOperator<S> crossoverOperator, MutationOperator<S> mutationOperator, SelectionOperator<List<S>, S> selectionOperator)
   :outertype: SteadyStateGeneticAlgorithm

   Constructor

Methods
-------
evaluatePopulation
^^^^^^^^^^^^^^^^^^

.. java:method:: @Override protected List<S> evaluatePopulation(List<S> population)
   :outertype: SteadyStateGeneticAlgorithm

getDescription
^^^^^^^^^^^^^^

.. java:method:: @Override public String getDescription()
   :outertype: SteadyStateGeneticAlgorithm

getName
^^^^^^^

.. java:method:: @Override public String getName()
   :outertype: SteadyStateGeneticAlgorithm

getResult
^^^^^^^^^

.. java:method:: @Override public S getResult()
   :outertype: SteadyStateGeneticAlgorithm

initProgress
^^^^^^^^^^^^

.. java:method:: @Override public void initProgress()
   :outertype: SteadyStateGeneticAlgorithm

isStoppingConditionReached
^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override protected boolean isStoppingConditionReached()
   :outertype: SteadyStateGeneticAlgorithm

replacement
^^^^^^^^^^^

.. java:method:: @Override protected List<S> replacement(List<S> population, List<S> offspringPopulation)
   :outertype: SteadyStateGeneticAlgorithm

reproduction
^^^^^^^^^^^^

.. java:method:: @Override protected List<S> reproduction(List<S> matingPopulation)
   :outertype: SteadyStateGeneticAlgorithm

selection
^^^^^^^^^

.. java:method:: @Override protected List<S> selection(List<S> population)
   :outertype: SteadyStateGeneticAlgorithm

updateProgress
^^^^^^^^^^^^^^

.. java:method:: @Override public void updateProgress()
   :outertype: SteadyStateGeneticAlgorithm

