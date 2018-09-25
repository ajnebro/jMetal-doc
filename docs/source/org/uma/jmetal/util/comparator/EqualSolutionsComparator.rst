.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: java.io Serializable

.. java:import:: java.util Comparator

EqualSolutionsComparator
========================

.. java:package:: org.uma.jmetal.util.comparator
   :noindex:

.. java:type:: @SuppressWarnings public class EqualSolutionsComparator<S extends Solution<?>> implements Comparator<S>, Serializable

   This class implements a \ ``Comparator``\  (a method for comparing \ ``Solution``\  objects) based whether all the objective values are equal or not. A dominance test is applied to decide about what solution is the best.

   :author: Antonio J. Nebro

Methods
-------
compare
^^^^^^^

.. java:method:: @Override public int compare(S solution1, S solution2)
   :outertype: EqualSolutionsComparator

   Compares two solutions.

   :param solution1: First \ ``Solution``\ .
   :param solution2: Second \ ``Solution``\ .
   :return: -1, or 0, or 1, or 2 if solution1 is dominates solution2, solution1 and solution2 are equals, or solution1 is greater than solution2, respectively.

