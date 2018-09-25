.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: java.io Serializable

.. java:import:: java.util Comparator

RankingAndCrowdingDistanceComparator
====================================

.. java:package:: org.uma.jmetal.util.comparator
   :noindex:

.. java:type:: @SuppressWarnings public class RankingAndCrowdingDistanceComparator<S extends Solution<?>> implements Comparator<S>, Serializable

   :author: Antonio J. Nebro

Methods
-------
compare
^^^^^^^

.. java:method:: @Override public int compare(S solution1, S solution2)
   :outertype: RankingAndCrowdingDistanceComparator

   Compares two solutions.

   :param solution1: Object representing the first solution
   :param solution2: Object representing the second solution.
   :return: -1, or 0, or 1 if solution1 is less than, equal, or greater than solution2, respectively.

