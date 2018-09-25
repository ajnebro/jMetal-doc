.. java:import:: org.uma.jmetal.algorithm Algorithm

.. java:import:: org.uma.jmetal.problem Problem

.. java:import:: java.util List

AbstractEvolutionaryAlgorithm
=============================

.. java:package:: org.uma.jmetal.algorithm.impl
   :noindex:

.. java:type:: @SuppressWarnings public abstract class AbstractEvolutionaryAlgorithm<S, R> implements Algorithm<R>

   Abstract class representing an evolutionary algorithm

   :author: Antonio J. Nebro
   :param <S>: Solution
   :param <R>: Result

Fields
------
population
^^^^^^^^^^

.. java:field:: protected List<S> population
   :outertype: AbstractEvolutionaryAlgorithm

problem
^^^^^^^

.. java:field:: protected Problem<S> problem
   :outertype: AbstractEvolutionaryAlgorithm

Methods
-------
createInitialPopulation
^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: protected abstract List<S> createInitialPopulation()
   :outertype: AbstractEvolutionaryAlgorithm

evaluatePopulation
^^^^^^^^^^^^^^^^^^

.. java:method:: protected abstract List<S> evaluatePopulation(List<S> population)
   :outertype: AbstractEvolutionaryAlgorithm

getPopulation
^^^^^^^^^^^^^

.. java:method:: public List<S> getPopulation()
   :outertype: AbstractEvolutionaryAlgorithm

getProblem
^^^^^^^^^^

.. java:method:: public Problem<S> getProblem()
   :outertype: AbstractEvolutionaryAlgorithm

getResult
^^^^^^^^^

.. java:method:: @Override public abstract R getResult()
   :outertype: AbstractEvolutionaryAlgorithm

initProgress
^^^^^^^^^^^^

.. java:method:: protected abstract void initProgress()
   :outertype: AbstractEvolutionaryAlgorithm

isStoppingConditionReached
^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: protected abstract boolean isStoppingConditionReached()
   :outertype: AbstractEvolutionaryAlgorithm

replacement
^^^^^^^^^^^

.. java:method:: protected abstract List<S> replacement(List<S> population, List<S> offspringPopulation)
   :outertype: AbstractEvolutionaryAlgorithm

reproduction
^^^^^^^^^^^^

.. java:method:: protected abstract List<S> reproduction(List<S> population)
   :outertype: AbstractEvolutionaryAlgorithm

run
^^^

.. java:method:: @Override public void run()
   :outertype: AbstractEvolutionaryAlgorithm

selection
^^^^^^^^^

.. java:method:: protected abstract List<S> selection(List<S> population)
   :outertype: AbstractEvolutionaryAlgorithm

setPopulation
^^^^^^^^^^^^^

.. java:method:: public void setPopulation(List<S> population)
   :outertype: AbstractEvolutionaryAlgorithm

setProblem
^^^^^^^^^^

.. java:method:: public void setProblem(Problem<S> problem)
   :outertype: AbstractEvolutionaryAlgorithm

updateProgress
^^^^^^^^^^^^^^

.. java:method:: protected abstract void updateProgress()
   :outertype: AbstractEvolutionaryAlgorithm

