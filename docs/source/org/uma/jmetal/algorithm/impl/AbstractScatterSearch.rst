.. java:import:: org.uma.jmetal.algorithm Algorithm

.. java:import:: java.util ArrayList

.. java:import:: java.util List

AbstractScatterSearch
=====================

.. java:package:: org.uma.jmetal.algorithm.impl
   :noindex:

.. java:type:: @SuppressWarnings public abstract class AbstractScatterSearch<S, R> implements Algorithm<R>

   Abstract class representing a scatter search algorithm

   :author: Antonio J. Nebro
   :param <S>: Solution
   :param <R>: Result

Methods
-------
diversificationGeneration
^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public abstract S diversificationGeneration()
   :outertype: AbstractScatterSearch

getPopulation
^^^^^^^^^^^^^

.. java:method:: public List<S> getPopulation()
   :outertype: AbstractScatterSearch

getPopulationSize
^^^^^^^^^^^^^^^^^

.. java:method:: public int getPopulationSize()
   :outertype: AbstractScatterSearch

getResult
^^^^^^^^^

.. java:method:: @Override public abstract R getResult()
   :outertype: AbstractScatterSearch

improvement
^^^^^^^^^^^

.. java:method:: public abstract S improvement(S solution)
   :outertype: AbstractScatterSearch

initializationPhase
^^^^^^^^^^^^^^^^^^^

.. java:method:: public void initializationPhase()
   :outertype: AbstractScatterSearch

   Initialization phase of the scatter search: the population is filled with diverse solutions that have been improved.

   :return: The population

isStoppingConditionReached
^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public abstract boolean isStoppingConditionReached()
   :outertype: AbstractScatterSearch

referenceSetUpdate
^^^^^^^^^^^^^^^^^^

.. java:method:: public abstract void referenceSetUpdate()
   :outertype: AbstractScatterSearch

referenceSetUpdate
^^^^^^^^^^^^^^^^^^

.. java:method:: public abstract void referenceSetUpdate(S solution)
   :outertype: AbstractScatterSearch

restart
^^^^^^^

.. java:method:: public abstract void restart()
   :outertype: AbstractScatterSearch

restartConditionIsFulfilled
^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public abstract boolean restartConditionIsFulfilled(List<S> solutionList)
   :outertype: AbstractScatterSearch

run
^^^

.. java:method:: @Override public void run()
   :outertype: AbstractScatterSearch

setPopulation
^^^^^^^^^^^^^

.. java:method:: public void setPopulation(List<S> population)
   :outertype: AbstractScatterSearch

setPopulationSize
^^^^^^^^^^^^^^^^^

.. java:method:: public void setPopulationSize(int populationSize)
   :outertype: AbstractScatterSearch

solutionCombination
^^^^^^^^^^^^^^^^^^^

.. java:method:: public abstract List<S> solutionCombination(List<List<S>> population)
   :outertype: AbstractScatterSearch

subsetGeneration
^^^^^^^^^^^^^^^^

.. java:method:: public abstract List<List<S>> subsetGeneration()
   :outertype: AbstractScatterSearch

