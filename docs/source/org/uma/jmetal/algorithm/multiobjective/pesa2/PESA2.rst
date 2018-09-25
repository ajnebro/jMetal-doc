.. java:import:: org.uma.jmetal.algorithm.impl AbstractGeneticAlgorithm

.. java:import:: org.uma.jmetal.algorithm.multiobjective.pesa2.util PESA2Selection

.. java:import:: org.uma.jmetal.operator CrossoverOperator

.. java:import:: org.uma.jmetal.operator MutationOperator

.. java:import:: org.uma.jmetal.operator SelectionOperator

.. java:import:: org.uma.jmetal.problem Problem

.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util.archive.impl AdaptiveGridArchive

.. java:import:: org.uma.jmetal.util.evaluator SolutionListEvaluator

.. java:import:: java.util ArrayList

.. java:import:: java.util Collections

.. java:import:: java.util List

PESA2
=====

.. java:package:: org.uma.jmetal.algorithm.multiobjective.pesa2
   :noindex:

.. java:type:: @SuppressWarnings public class PESA2<S extends Solution<?>> extends AbstractGeneticAlgorithm<S, List<S>>

   :author: Antonio J. Nebro

Fields
------
evaluator
^^^^^^^^^

.. java:field:: protected final SolutionListEvaluator<S> evaluator
   :outertype: PESA2

selectionOperator
^^^^^^^^^^^^^^^^^

.. java:field:: protected SelectionOperator<AdaptiveGridArchive<S>, S> selectionOperator
   :outertype: PESA2

Constructors
------------
PESA2
^^^^^

.. java:constructor:: public PESA2(Problem<S> problem, int maxEvaluations, int populationSize, int archiveSize, int biSections, CrossoverOperator<S> crossoverOperator, MutationOperator<S> mutationOperator, SolutionListEvaluator<S> evaluator)
   :outertype: PESA2

Methods
-------
evaluatePopulation
^^^^^^^^^^^^^^^^^^

.. java:method:: @Override protected List<S> evaluatePopulation(List<S> population)
   :outertype: PESA2

getDescription
^^^^^^^^^^^^^^

.. java:method:: @Override public String getDescription()
   :outertype: PESA2

getName
^^^^^^^

.. java:method:: @Override public String getName()
   :outertype: PESA2

getResult
^^^^^^^^^

.. java:method:: @Override public List<S> getResult()
   :outertype: PESA2

initProgress
^^^^^^^^^^^^

.. java:method:: @Override protected void initProgress()
   :outertype: PESA2

isStoppingConditionReached
^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override protected boolean isStoppingConditionReached()
   :outertype: PESA2

replacement
^^^^^^^^^^^

.. java:method:: @Override protected List<S> replacement(List<S> population, List<S> offspringPopulation)
   :outertype: PESA2

reproduction
^^^^^^^^^^^^

.. java:method:: @Override protected List<S> reproduction(List<S> population)
   :outertype: PESA2

selection
^^^^^^^^^

.. java:method:: @Override protected List<S> selection(List<S> population)
   :outertype: PESA2

updateProgress
^^^^^^^^^^^^^^

.. java:method:: @Override protected void updateProgress()
   :outertype: PESA2

