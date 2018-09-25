.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util.solutionattribute.impl CrowdingDistance

.. java:import:: java.io Serializable

.. java:import:: java.util Comparator

CrowdingDistanceComparator
==========================

.. java:package:: org.uma.jmetal.util.comparator
   :noindex:

.. java:type:: @SuppressWarnings public class CrowdingDistanceComparator<S extends Solution<?>> implements Comparator<S>, Serializable

   Compares two solutions according to the crowding distance attribute. The higher the distance the better

   :author: Antonio J. Nebro

Methods
-------
compare
^^^^^^^

.. java:method:: @Override public int compare(S solution1, S solution2)
   :outertype: CrowdingDistanceComparator

   Compare two solutions.

   :param solution1: Object representing the first \ ``Solution``\ .
   :param solution2: Object representing the second \ ``Solution``\ .
   :return: -1, or 0, or 1 if solution1 is has greater, equal, or less distance value than solution2, respectively.

