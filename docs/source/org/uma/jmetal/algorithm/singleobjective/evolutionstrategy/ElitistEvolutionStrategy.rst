.. java:import:: org.uma.jmetal.algorithm.impl AbstractEvolutionStrategy

.. java:import:: org.uma.jmetal.operator MutationOperator

.. java:import:: org.uma.jmetal.problem Problem

.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util.comparator ObjectiveComparator

.. java:import:: java.util ArrayList

.. java:import:: java.util Collections

.. java:import:: java.util Comparator

.. java:import:: java.util List

ElitistEvolutionStrategy
========================

.. java:package:: org.uma.jmetal.algorithm.singleobjective.evolutionstrategy
   :noindex:

.. java:type:: @SuppressWarnings public class ElitistEvolutionStrategy<S extends Solution<?>> extends AbstractEvolutionStrategy<S, S>

   Class implementing a (mu + lambda) Evolution Strategy (lambda must be divisible by mu)

   :author: Antonio J. Nebro

Constructors
------------
ElitistEvolutionStrategy
^^^^^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public ElitistEvolutionStrategy(Problem<S> problem, int mu, int lambda, int maxEvaluations, MutationOperator<S> mutation)
   :outertype: ElitistEvolutionStrategy

   Constructor

Methods
-------
createInitialPopulation
^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override protected List<S> createInitialPopulation()
   :outertype: ElitistEvolutionStrategy

evaluatePopulation
^^^^^^^^^^^^^^^^^^

.. java:method:: @Override protected List<S> evaluatePopulation(List<S> population)
   :outertype: ElitistEvolutionStrategy

getDescription
^^^^^^^^^^^^^^

.. java:method:: @Override public String getDescription()
   :outertype: ElitistEvolutionStrategy

getName
^^^^^^^

.. java:method:: @Override public String getName()
   :outertype: ElitistEvolutionStrategy

getResult
^^^^^^^^^

.. java:method:: @Override public S getResult()
   :outertype: ElitistEvolutionStrategy

initProgress
^^^^^^^^^^^^

.. java:method:: @Override protected void initProgress()
   :outertype: ElitistEvolutionStrategy

isStoppingConditionReached
^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override protected boolean isStoppingConditionReached()
   :outertype: ElitistEvolutionStrategy

replacement
^^^^^^^^^^^

.. java:method:: @Override protected List<S> replacement(List<S> population, List<S> offspringPopulation)
   :outertype: ElitistEvolutionStrategy

reproduction
^^^^^^^^^^^^

.. java:method:: @SuppressWarnings @Override protected List<S> reproduction(List<S> population)
   :outertype: ElitistEvolutionStrategy

selection
^^^^^^^^^

.. java:method:: @Override protected List<S> selection(List<S> population)
   :outertype: ElitistEvolutionStrategy

updateProgress
^^^^^^^^^^^^^^

.. java:method:: @Override protected void updateProgress()
   :outertype: ElitistEvolutionStrategy

