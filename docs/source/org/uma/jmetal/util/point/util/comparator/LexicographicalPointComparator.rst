.. java:import:: java.util Comparator

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: org.uma.jmetal.util.point Point

LexicographicalPointComparator
==============================

.. java:package:: org.uma.jmetal.util.point.util.comparator
   :noindex:

.. java:type:: public class LexicographicalPointComparator implements Comparator<Point>

   This class implements the Comparator interface for comparing tow points. The order used is lexicographical order.

   :author: Antonio J. Nebro , Juan J. Durillo

Methods
-------
compare
^^^^^^^

.. java:method:: @Override public int compare(Point pointOne, Point pointTwo)
   :outertype: LexicographicalPointComparator

   The compare method compare the objects o1 and o2.

   :param pointOne: An object that reference a double[]
   :param pointTwo: An object that reference a double[]
   :return: The following value: -1 if point1 < point2, 1 if point1 > point2 or 0 in other case.

