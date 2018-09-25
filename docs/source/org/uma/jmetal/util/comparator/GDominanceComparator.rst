.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: java.io Serializable

.. java:import:: java.util Comparator

.. java:import:: java.util List

GDominanceComparator
====================

.. java:package:: org.uma.jmetal.util.comparator
   :noindex:

.. java:type:: @SuppressWarnings public class GDominanceComparator<S extends Solution<?>> implements Comparator<S>, Serializable

   This class implements a solution comparator according to the concept of g-dominance (https://doi.org/10.1016/j.ejor.2008.07.015)

   :author: Antonio J. Nebro

Constructors
------------
GDominanceComparator
^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public GDominanceComparator(List<Double> referencePoint)
   :outertype: GDominanceComparator

   Constructor

Methods
-------
compare
^^^^^^^

.. java:method:: @Override public int compare(S solution1, S solution2)
   :outertype: GDominanceComparator

   Compares two solutions.

   :param solution1: Object representing the first \ ``Solution``\ .
   :param solution2: Object representing the second \ ``Solution``\ .
   :return: -1, or 0, or 1 if solution1 dominates solution2, both are non-dominated, or solution1 is dominated by solution2, respectively.

