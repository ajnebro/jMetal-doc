.. java:import:: org.uma.jmetal.operator CrossoverOperator

.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: java.util List

TwoPointCrossover
=================

.. java:package:: org.uma.jmetal.operator.impl.crossover
   :noindex:

.. java:type:: public class TwoPointCrossover<T> implements CrossoverOperator<Solution<T>>

   Created by FlapKap on 27-05-2017.

Fields
------
operator
^^^^^^^^

.. java:field::  NPointCrossover<T> operator
   :outertype: TwoPointCrossover

Constructors
------------
TwoPointCrossover
^^^^^^^^^^^^^^^^^

.. java:constructor:: public TwoPointCrossover(double probability)
   :outertype: TwoPointCrossover

Methods
-------
execute
^^^^^^^

.. java:method:: @Override public List<Solution<T>> execute(List<Solution<T>> solutions)
   :outertype: TwoPointCrossover

getCrossoverProbability
^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public double getCrossoverProbability()
   :outertype: TwoPointCrossover

getNumberOfGeneratedChildren
^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public int getNumberOfGeneratedChildren()
   :outertype: TwoPointCrossover

getNumberOfRequiredParents
^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public int getNumberOfRequiredParents()
   :outertype: TwoPointCrossover

