.. java:import:: org.uma.jmetal.algorithm.impl AbstractGeneticAlgorithm

.. java:import:: org.uma.jmetal.operator CrossoverOperator

.. java:import:: org.uma.jmetal.operator MutationOperator

.. java:import:: org.uma.jmetal.operator SelectionOperator

.. java:import:: org.uma.jmetal.problem Problem

.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util.comparator ObjectiveComparator

.. java:import:: org.uma.jmetal.util.evaluator SolutionListEvaluator

.. java:import:: java.util Collections

.. java:import:: java.util Comparator

.. java:import:: java.util List

GenerationalGeneticAlgorithm
============================

.. java:package:: org.uma.jmetal.algorithm.singleobjective.geneticalgorithm
   :noindex:

.. java:type:: @SuppressWarnings public class GenerationalGeneticAlgorithm<S extends Solution<?>> extends AbstractGeneticAlgorithm<S, S>

   :author: Antonio J. Nebro

Constructors
------------
GenerationalGeneticAlgorithm
^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public GenerationalGeneticAlgorithm(Problem<S> problem, int maxEvaluations, int populationSize, CrossoverOperator<S> crossoverOperator, MutationOperator<S> mutationOperator, SelectionOperator<List<S>, S> selectionOperator, SolutionListEvaluator<S> evaluator)
   :outertype: GenerationalGeneticAlgorithm

   Constructor

Methods
-------
evaluatePopulation
^^^^^^^^^^^^^^^^^^

.. java:method:: @Override protected List<S> evaluatePopulation(List<S> population)
   :outertype: GenerationalGeneticAlgorithm

getDescription
^^^^^^^^^^^^^^

.. java:method:: @Override public String getDescription()
   :outertype: GenerationalGeneticAlgorithm

getName
^^^^^^^

.. java:method:: @Override public String getName()
   :outertype: GenerationalGeneticAlgorithm

getResult
^^^^^^^^^

.. java:method:: @Override public S getResult()
   :outertype: GenerationalGeneticAlgorithm

initProgress
^^^^^^^^^^^^

.. java:method:: @Override public void initProgress()
   :outertype: GenerationalGeneticAlgorithm

isStoppingConditionReached
^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override protected boolean isStoppingConditionReached()
   :outertype: GenerationalGeneticAlgorithm

replacement
^^^^^^^^^^^

.. java:method:: @Override protected List<S> replacement(List<S> population, List<S> offspringPopulation)
   :outertype: GenerationalGeneticAlgorithm

updateProgress
^^^^^^^^^^^^^^

.. java:method:: @Override public void updateProgress()
   :outertype: GenerationalGeneticAlgorithm

