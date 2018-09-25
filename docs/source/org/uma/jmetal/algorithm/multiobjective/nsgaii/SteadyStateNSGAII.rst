.. java:import:: org.uma.jmetal.operator CrossoverOperator

.. java:import:: org.uma.jmetal.operator MutationOperator

.. java:import:: org.uma.jmetal.operator SelectionOperator

.. java:import:: org.uma.jmetal.problem Problem

.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util.evaluator SolutionListEvaluator

.. java:import:: java.util ArrayList

.. java:import:: java.util Comparator

.. java:import:: java.util List

SteadyStateNSGAII
=================

.. java:package:: org.uma.jmetal.algorithm.multiobjective.nsgaii
   :noindex:

.. java:type:: @SuppressWarnings public class SteadyStateNSGAII<S extends Solution<?>> extends NSGAII<S>

   :author: Antonio J. Nebro

Constructors
------------
SteadyStateNSGAII
^^^^^^^^^^^^^^^^^

.. java:constructor:: public SteadyStateNSGAII(Problem<S> problem, int maxEvaluations, int populationSize, CrossoverOperator<S> crossoverOperator, MutationOperator<S> mutationOperator, SelectionOperator<List<S>, S> selectionOperator, Comparator<S> dominanceComparator, SolutionListEvaluator<S> evaluator)
   :outertype: SteadyStateNSGAII

   Constructor

Methods
-------
getDescription
^^^^^^^^^^^^^^

.. java:method:: @Override public String getDescription()
   :outertype: SteadyStateNSGAII

getName
^^^^^^^

.. java:method:: @Override public String getName()
   :outertype: SteadyStateNSGAII

reproduction
^^^^^^^^^^^^

.. java:method:: @Override protected List<S> reproduction(List<S> population)
   :outertype: SteadyStateNSGAII

selection
^^^^^^^^^

.. java:method:: @Override protected List<S> selection(List<S> population)
   :outertype: SteadyStateNSGAII

updateProgress
^^^^^^^^^^^^^^

.. java:method:: @Override protected void updateProgress()
   :outertype: SteadyStateNSGAII

