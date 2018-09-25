.. java:import:: java.util Comparator

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: org.uma.jmetal.util.point Point

PointComparator
===============

.. java:package:: org.uma.jmetal.util.point.util.comparator
   :noindex:

.. java:type:: public class PointComparator implements Comparator<Point>

   Point comparator. Starts the comparison from front last point dimension to the first one

   :author: Antonio J. Nebro

Constructors
------------
PointComparator
^^^^^^^^^^^^^^^

.. java:constructor:: public PointComparator()
   :outertype: PointComparator

Methods
-------
compare
^^^^^^^

.. java:method:: @Override public int compare(Point pointOne, Point pointTwo)
   :outertype: PointComparator

   Compares two Point objects

   :param pointOne: An object that reference a Point
   :param pointTwo: An object that reference a Point
   :return: -1 if o1 < o1, 1 if o1 > o2 or 0 in other case.

setMaximizing
^^^^^^^^^^^^^

.. java:method:: public void setMaximizing()
   :outertype: PointComparator

setMinimizing
^^^^^^^^^^^^^

.. java:method:: public void setMinimizing()
   :outertype: PointComparator

