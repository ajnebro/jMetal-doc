.. java:import:: org.uma.jmetal.algorithm.impl AbstractGeneticAlgorithm

.. java:import:: org.uma.jmetal.operator CrossoverOperator

.. java:import:: org.uma.jmetal.operator MutationOperator

.. java:import:: org.uma.jmetal.operator SelectionOperator

.. java:import:: org.uma.jmetal.problem Problem

.. java:import:: org.uma.jmetal.qualityindicator.impl Hypervolume

.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util.solutionattribute Ranking

.. java:import:: org.uma.jmetal.util.solutionattribute.impl DominanceRanking

.. java:import:: java.util ArrayList

.. java:import:: java.util Comparator

.. java:import:: java.util List

SMSEMOA
=======

.. java:package:: org.uma.jmetal.algorithm.multiobjective.smsemoa
   :noindex:

.. java:type:: @SuppressWarnings public class SMSEMOA<S extends Solution<?>> extends AbstractGeneticAlgorithm<S, List<S>>

   :author: Antonio J. Nebro

Fields
------
dominanceComparator
^^^^^^^^^^^^^^^^^^^

.. java:field:: protected Comparator<S> dominanceComparator
   :outertype: SMSEMOA

evaluations
^^^^^^^^^^^

.. java:field:: protected int evaluations
   :outertype: SMSEMOA

maxEvaluations
^^^^^^^^^^^^^^

.. java:field:: protected final int maxEvaluations
   :outertype: SMSEMOA

offset
^^^^^^

.. java:field:: protected final double offset
   :outertype: SMSEMOA

Constructors
------------
SMSEMOA
^^^^^^^

.. java:constructor:: public SMSEMOA(Problem<S> problem, int maxEvaluations, int populationSize, double offset, CrossoverOperator<S> crossoverOperator, MutationOperator<S> mutationOperator, SelectionOperator<List<S>, S> selectionOperator, Comparator<S> dominanceComparator, Hypervolume<S> hypervolumeImplementation)
   :outertype: SMSEMOA

   Constructor

Methods
-------
computeRanking
^^^^^^^^^^^^^^

.. java:method:: protected Ranking<S> computeRanking(List<S> solutionList)
   :outertype: SMSEMOA

evaluatePopulation
^^^^^^^^^^^^^^^^^^

.. java:method:: @Override protected List<S> evaluatePopulation(List<S> population)
   :outertype: SMSEMOA

getDescription
^^^^^^^^^^^^^^

.. java:method:: @Override public String getDescription()
   :outertype: SMSEMOA

getName
^^^^^^^

.. java:method:: @Override public String getName()
   :outertype: SMSEMOA

getResult
^^^^^^^^^

.. java:method:: @Override public List<S> getResult()
   :outertype: SMSEMOA

initProgress
^^^^^^^^^^^^

.. java:method:: @Override protected void initProgress()
   :outertype: SMSEMOA

isStoppingConditionReached
^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override protected boolean isStoppingConditionReached()
   :outertype: SMSEMOA

replacement
^^^^^^^^^^^

.. java:method:: @Override protected List<S> replacement(List<S> population, List<S> offspringPopulation)
   :outertype: SMSEMOA

reproduction
^^^^^^^^^^^^

.. java:method:: @Override protected List<S> reproduction(List<S> population)
   :outertype: SMSEMOA

selection
^^^^^^^^^

.. java:method:: @Override protected List<S> selection(List<S> population)
   :outertype: SMSEMOA

updateProgress
^^^^^^^^^^^^^^

.. java:method:: @Override protected void updateProgress()
   :outertype: SMSEMOA

