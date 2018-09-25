.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util.solutionattribute.impl Fitness

.. java:import:: java.io Serializable

.. java:import:: java.util Comparator

FitnessComparator
=================

.. java:package:: org.uma.jmetal.util.comparator
   :noindex:

.. java:type:: @SuppressWarnings public class FitnessComparator<S extends Solution<?>> implements Comparator<S>, Serializable

   This class implements a \ ``Comparator``\  (a method for comparing \ ``Solution``\  objects) based on the fitness value returned by the method \ ``getFitness``\ .

   :author: Antonio J. Nebro

Methods
-------
compare
^^^^^^^

.. java:method:: @Override public int compare(S solution1, S solution2)
   :outertype: FitnessComparator

   Compares two solutions.

   :param solution1: Object representing the first \ ``Solution``\ .
   :param solution2: Object representing the second \ ``Solution``\ .
   :return: -1, or 0, or 1 if o1 is less than, equal, or greater than o2, respectively.

