.. java:import:: org.uma.jmetal.problem Problem

.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util AlgorithmBuilder

RandomSearchBuilder
===================

.. java:package:: org.uma.jmetal.algorithm.multiobjective.randomsearch
   :noindex:

.. java:type:: public class RandomSearchBuilder<S extends Solution<?>> implements AlgorithmBuilder<RandomSearch<S>>

   This class implements a simple random search algorithm.

   :author: Antonio J. Nebro

Constructors
------------
RandomSearchBuilder
^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public RandomSearchBuilder(Problem<S> problem)
   :outertype: RandomSearchBuilder

Methods
-------
build
^^^^^

.. java:method:: public RandomSearch<S> build()
   :outertype: RandomSearchBuilder

getMaxEvaluations
^^^^^^^^^^^^^^^^^

.. java:method:: public int getMaxEvaluations()
   :outertype: RandomSearchBuilder

setMaxEvaluations
^^^^^^^^^^^^^^^^^

.. java:method:: public RandomSearchBuilder<S> setMaxEvaluations(int maxEvaluations)
   :outertype: RandomSearchBuilder

