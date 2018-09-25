.. java:import:: org.uma.jmetal.algorithm Algorithm

.. java:import:: org.uma.jmetal.problem Problem

.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util.archive.impl NonDominatedSolutionListArchive

.. java:import:: java.util List

RandomSearch
============

.. java:package:: org.uma.jmetal.algorithm.multiobjective.randomsearch
   :noindex:

.. java:type:: @SuppressWarnings public class RandomSearch<S extends Solution<?>> implements Algorithm<List<S>>

   This class implements a simple random search algorithm.

   :author: Antonio J. Nebro

Fields
------
nonDominatedArchive
^^^^^^^^^^^^^^^^^^^

.. java:field::  NonDominatedSolutionListArchive<S> nonDominatedArchive
   :outertype: RandomSearch

Constructors
------------
RandomSearch
^^^^^^^^^^^^

.. java:constructor:: public RandomSearch(Problem<S> problem, int maxEvaluations)
   :outertype: RandomSearch

   Constructor

Methods
-------
getDescription
^^^^^^^^^^^^^^

.. java:method:: @Override public String getDescription()
   :outertype: RandomSearch

getMaxEvaluations
^^^^^^^^^^^^^^^^^

.. java:method:: public int getMaxEvaluations()
   :outertype: RandomSearch

getName
^^^^^^^

.. java:method:: @Override public String getName()
   :outertype: RandomSearch

getResult
^^^^^^^^^

.. java:method:: @Override public List<S> getResult()
   :outertype: RandomSearch

run
^^^

.. java:method:: @Override public void run()
   :outertype: RandomSearch

