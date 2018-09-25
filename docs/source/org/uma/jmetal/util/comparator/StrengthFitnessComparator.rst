.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util.solutionattribute.impl StrengthRawFitness

.. java:import:: java.io Serializable

.. java:import:: java.util Comparator

StrengthFitnessComparator
=========================

.. java:package:: org.uma.jmetal.util.comparator
   :noindex:

.. java:type:: @SuppressWarnings public class StrengthFitnessComparator<S extends Solution<?>> implements Comparator<S>, Serializable

   :author: Juan J. Durillo
   :param <S>:

Methods
-------
compare
^^^^^^^

.. java:method:: @Override public int compare(S solution1, S solution2)
   :outertype: StrengthFitnessComparator

