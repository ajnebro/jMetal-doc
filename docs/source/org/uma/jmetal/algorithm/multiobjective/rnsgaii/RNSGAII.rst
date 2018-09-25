.. java:import:: org.uma.jmetal.algorithm InteractiveAlgorithm

.. java:import:: org.uma.jmetal.algorithm.multiobjective.nsgaii NSGAII

.. java:import:: org.uma.jmetal.operator CrossoverOperator

.. java:import:: org.uma.jmetal.operator MutationOperator

.. java:import:: org.uma.jmetal.operator SelectionOperator

.. java:import:: org.uma.jmetal.operator.impl.selection RankingAndPreferenceSelection

.. java:import:: org.uma.jmetal.problem Problem

.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util.comparator DominanceComparator

.. java:import:: org.uma.jmetal.util.evaluator SolutionListEvaluator

.. java:import:: java.util ArrayList

.. java:import:: java.util List

RNSGAII
=======

.. java:package:: org.uma.jmetal.algorithm.multiobjective.rnsgaii
   :noindex:

.. java:type:: @SuppressWarnings public class RNSGAII<S extends Solution<?>> extends NSGAII<S> implements InteractiveAlgorithm<S, List<S>>

   :author: Antonio J. Nebro

Constructors
------------
RNSGAII
^^^^^^^

.. java:constructor:: public RNSGAII(Problem<S> problem, int maxEvaluations, int populationSize, CrossoverOperator<S> crossoverOperator, MutationOperator<S> mutationOperator, SelectionOperator<List<S>, S> selectionOperator, SolutionListEvaluator<S> evaluator, List<Double> interestPoint, double epsilon)
   :outertype: RNSGAII

   Constructor

Methods
-------
getDescription
^^^^^^^^^^^^^^

.. java:method:: @Override public String getDescription()
   :outertype: RNSGAII

getName
^^^^^^^

.. java:method:: @Override public String getName()
   :outertype: RNSGAII

getResult
^^^^^^^^^

.. java:method:: @Override public List<S> getResult()
   :outertype: RNSGAII

initProgress
^^^^^^^^^^^^

.. java:method:: @Override protected void initProgress()
   :outertype: RNSGAII

isStoppingConditionReached
^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override protected boolean isStoppingConditionReached()
   :outertype: RNSGAII

replacement
^^^^^^^^^^^

.. java:method:: @Override protected List<S> replacement(List<S> population, List<S> offspringPopulation)
   :outertype: RNSGAII

updatePointOfInterest
^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public void updatePointOfInterest(List<Double> newReferencePoints)
   :outertype: RNSGAII

updateProgress
^^^^^^^^^^^^^^

.. java:method:: @Override protected void updateProgress()
   :outertype: RNSGAII

