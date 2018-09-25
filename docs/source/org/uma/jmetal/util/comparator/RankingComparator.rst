.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util.solutionattribute Ranking

.. java:import:: org.uma.jmetal.util.solutionattribute.impl DominanceRanking

.. java:import:: java.io Serializable

.. java:import:: java.util Comparator

RankingComparator
=================

.. java:package:: org.uma.jmetal.util.comparator
   :noindex:

.. java:type:: @SuppressWarnings public class RankingComparator<S extends Solution<?>> implements Comparator<S>, Serializable

   :author: Antonio J. Nebro This class implements a comparator based on the rank of the solutions.

Methods
-------
compare
^^^^^^^

.. java:method:: @Override public int compare(S solution1, S solution2)
   :outertype: RankingComparator

   Compares two solutions according to the ranking attribute. The lower the ranking the better

   :param solution1: Object representing the first solution.
   :param solution2: Object representing the second solution.
   :return: -1, or 0, or 1 if o1 is less than, equal, or greater than o2, respectively.

