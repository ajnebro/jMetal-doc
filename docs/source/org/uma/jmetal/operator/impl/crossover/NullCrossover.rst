.. java:import:: org.uma.jmetal.operator CrossoverOperator

.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: java.util ArrayList

.. java:import:: java.util List

NullCrossover
=============

.. java:package:: org.uma.jmetal.operator.impl.crossover
   :noindex:

.. java:type:: @SuppressWarnings public class NullCrossover<S extends Solution<?>> implements CrossoverOperator<S>

   This class defines a null crossover operator: the parent solutions are returned without any change. It can be useful when configuring a genetic algorithm and we want to use only mutation.

   :author: Antonio J. Nebro

Methods
-------
execute
^^^^^^^

.. java:method:: @Override public List<S> execute(List<S> source)
   :outertype: NullCrossover

   Execute() method

getNumberOfGeneratedChildren
^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public int getNumberOfGeneratedChildren()
   :outertype: NullCrossover

getNumberOfRequiredParents
^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public int getNumberOfRequiredParents()
   :outertype: NullCrossover

