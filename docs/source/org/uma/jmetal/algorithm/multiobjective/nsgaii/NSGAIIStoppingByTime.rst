.. java:import:: org.uma.jmetal.operator CrossoverOperator

.. java:import:: org.uma.jmetal.operator MutationOperator

.. java:import:: org.uma.jmetal.operator SelectionOperator

.. java:import:: org.uma.jmetal.problem ConstrainedProblem

.. java:import:: org.uma.jmetal.problem Problem

.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: java.util Comparator

.. java:import:: java.util List

NSGAIIStoppingByTime
====================

.. java:package:: org.uma.jmetal.algorithm.multiobjective.nsgaii
   :noindex:

.. java:type:: @SuppressWarnings public class NSGAIIStoppingByTime<S extends Solution<?>> extends NSGAII<S>

   This class shows a version of NSGA-II having a stopping condition depending on run-time

   :author: Antonio J. Nebro

Constructors
------------
NSGAIIStoppingByTime
^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public NSGAIIStoppingByTime(Problem<S> problem, int populationSize, long maxComputingTime, CrossoverOperator<S> crossoverOperator, MutationOperator<S> mutationOperator, SelectionOperator<List<S>, S> selectionOperator, Comparator<S> dominanceComparator)
   :outertype: NSGAIIStoppingByTime

   Constructor

Methods
-------
evaluatePopulation
^^^^^^^^^^^^^^^^^^

.. java:method:: @Override protected List<S> evaluatePopulation(List<S> population)
   :outertype: NSGAIIStoppingByTime

getDescription
^^^^^^^^^^^^^^

.. java:method:: @Override public String getDescription()
   :outertype: NSGAIIStoppingByTime

getName
^^^^^^^

.. java:method:: @Override public String getName()
   :outertype: NSGAIIStoppingByTime

initProgress
^^^^^^^^^^^^

.. java:method:: @Override protected void initProgress()
   :outertype: NSGAIIStoppingByTime

isStoppingConditionReached
^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override protected boolean isStoppingConditionReached()
   :outertype: NSGAIIStoppingByTime

updateProgress
^^^^^^^^^^^^^^

.. java:method:: @Override protected void updateProgress()
   :outertype: NSGAIIStoppingByTime

