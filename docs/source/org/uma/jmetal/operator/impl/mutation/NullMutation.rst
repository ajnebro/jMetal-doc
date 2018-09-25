.. java:import:: org.uma.jmetal.operator MutationOperator

NullMutation
============

.. java:package:: org.uma.jmetal.operator.impl.mutation
   :noindex:

.. java:type:: @SuppressWarnings public class NullMutation<S> implements MutationOperator<S>

   This class is intended to perform no mutation. It can be useful when configuring a genetic algorithm and we want to use only crossover.

   :author: Antonio J. Nebro

Methods
-------
execute
^^^^^^^

.. java:method:: @Override public S execute(S source)
   :outertype: NullMutation

   Execute() method

