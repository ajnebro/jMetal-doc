.. java:import:: org.uma.jmetal.operator MutationOperator

.. java:import:: org.uma.jmetal.problem Problem

AbstractEvolutionStrategy
=========================

.. java:package:: org.uma.jmetal.algorithm.impl
   :noindex:

.. java:type:: @SuppressWarnings public abstract class AbstractEvolutionStrategy<S, Result> extends AbstractEvolutionaryAlgorithm<S, Result>

   Abstract class representing an evolution strategy algorithm

   :author: Antonio J. Nebro

Fields
------
mutationOperator
^^^^^^^^^^^^^^^^

.. java:field:: protected MutationOperator<S> mutationOperator
   :outertype: AbstractEvolutionStrategy

Constructors
------------
AbstractEvolutionStrategy
^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public AbstractEvolutionStrategy(Problem<S> problem)
   :outertype: AbstractEvolutionStrategy

   Constructor

   :param problem: The problem to solve

Methods
-------
getMutationOperator
^^^^^^^^^^^^^^^^^^^

.. java:method:: public MutationOperator<S> getMutationOperator()
   :outertype: AbstractEvolutionStrategy

