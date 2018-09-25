.. java:import:: org.apache.commons.lang3 ArrayUtils

.. java:import:: org.uma.jmetal.operator CrossoverOperator

.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: org.uma.jmetal.util.pseudorandom JMetalRandom

.. java:import:: java.util ArrayList

.. java:import:: java.util List

NPointCrossover
===============

.. java:package:: org.uma.jmetal.operator.impl.crossover
   :noindex:

.. java:type:: public class NPointCrossover<T> implements CrossoverOperator<Solution<T>>

   Created by FlapKap on 23-03-2017.

Constructors
------------
NPointCrossover
^^^^^^^^^^^^^^^

.. java:constructor:: public NPointCrossover(double probability, int crossovers)
   :outertype: NPointCrossover

NPointCrossover
^^^^^^^^^^^^^^^

.. java:constructor:: public NPointCrossover(int crossovers)
   :outertype: NPointCrossover

Methods
-------
execute
^^^^^^^

.. java:method:: @Override public List<Solution<T>> execute(List<Solution<T>> s)
   :outertype: NPointCrossover

getCrossoverProbability
^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public double getCrossoverProbability()
   :outertype: NPointCrossover

getNumberOfGeneratedChildren
^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public int getNumberOfGeneratedChildren()
   :outertype: NPointCrossover

getNumberOfRequiredParents
^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public int getNumberOfRequiredParents()
   :outertype: NPointCrossover

