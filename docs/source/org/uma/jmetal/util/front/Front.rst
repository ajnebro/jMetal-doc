.. java:import:: org.uma.jmetal.util.point Point

.. java:import:: java.io Serializable

.. java:import:: java.util Comparator

Front
=====

.. java:package:: org.uma.jmetal.util.front
   :noindex:

.. java:type:: public interface Front extends Serializable

   A front is a list of points

   :author: Antonio J. Nebro

Methods
-------
getNumberOfPoints
^^^^^^^^^^^^^^^^^

.. java:method:: public int getNumberOfPoints()
   :outertype: Front

getPoint
^^^^^^^^

.. java:method:: public Point getPoint(int index)
   :outertype: Front

getPointDimensions
^^^^^^^^^^^^^^^^^^

.. java:method:: public int getPointDimensions()
   :outertype: Front

setPoint
^^^^^^^^

.. java:method:: public void setPoint(int index, Point point)
   :outertype: Front

sort
^^^^

.. java:method:: public void sort(Comparator<Point> comparator)
   :outertype: Front

