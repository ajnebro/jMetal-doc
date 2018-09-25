.. java:import:: java.util Comparator

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: org.uma.jmetal.util.point Point

PointDimensionComparator
========================

.. java:package:: org.uma.jmetal.util.point.util.comparator
   :noindex:

.. java:type:: public class PointDimensionComparator implements Comparator<Point>

   This class implements the \ :java:ref:`Comparator`\  interface. It is used to compare two points according the value of a particular dimension.

   :author: Antonio J. Nebro , Juan J. Durillo

Constructors
------------
PointDimensionComparator
^^^^^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public PointDimensionComparator(int index)
   :outertype: PointDimensionComparator

   Constructor

Methods
-------
compare
^^^^^^^

.. java:method:: @Override public int compare(Point pointOne, Point pointTwo)
   :outertype: PointDimensionComparator

   Compares the objects o1 and o2.

   :param pointOne: An object that reference a double[]
   :param pointTwo: An object that reference a double[]
   :return: -1 if o1 < o1, 1 if o1 > o2 or 0 in other case.

