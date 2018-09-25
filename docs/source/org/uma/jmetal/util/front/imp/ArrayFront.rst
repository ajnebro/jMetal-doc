.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: org.uma.jmetal.util.front Front

.. java:import:: org.uma.jmetal.util.point Point

.. java:import:: org.uma.jmetal.util.point.impl ArrayPoint

ArrayFront
==========

.. java:package:: org.uma.jmetal.util.front.imp
   :noindex:

.. java:type:: @SuppressWarnings public class ArrayFront implements Front

   This class implements the \ :java:ref:`Front`\  interface by using an array of \ :java:ref:`Point`\  objects

   :author: Antonio J. Nebro

Fields
------
numberOfPoints
^^^^^^^^^^^^^^

.. java:field:: protected int numberOfPoints
   :outertype: ArrayFront

points
^^^^^^

.. java:field:: protected Point[] points
   :outertype: ArrayFront

Constructors
------------
ArrayFront
^^^^^^^^^^

.. java:constructor:: public ArrayFront()
   :outertype: ArrayFront

   Constructor

ArrayFront
^^^^^^^^^^

.. java:constructor:: public ArrayFront(List<? extends Solution<?>> solutionList)
   :outertype: ArrayFront

   Constructor

ArrayFront
^^^^^^^^^^

.. java:constructor:: public ArrayFront(Front front)
   :outertype: ArrayFront

   Copy Constructor

ArrayFront
^^^^^^^^^^

.. java:constructor:: public ArrayFront(int numberOfPoints, int dimensions)
   :outertype: ArrayFront

   Constructor

ArrayFront
^^^^^^^^^^

.. java:constructor:: public ArrayFront(String fileName) throws FileNotFoundException
   :outertype: ArrayFront

   Constructor

   :param fileName: File containing the data. Each line of the file is a list of objective values
   :throws FileNotFoundException:

Methods
-------
createInputStream
^^^^^^^^^^^^^^^^^

.. java:method:: public InputStream createInputStream(String fileName) throws FileNotFoundException
   :outertype: ArrayFront

equals
^^^^^^

.. java:method:: @Override public boolean equals(Object o)
   :outertype: ArrayFront

getNumberOfPoints
^^^^^^^^^^^^^^^^^

.. java:method:: @Override public int getNumberOfPoints()
   :outertype: ArrayFront

getPoint
^^^^^^^^

.. java:method:: @Override public Point getPoint(int index)
   :outertype: ArrayFront

getPointDimensions
^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public int getPointDimensions()
   :outertype: ArrayFront

hashCode
^^^^^^^^

.. java:method:: @Override public int hashCode()
   :outertype: ArrayFront

setPoint
^^^^^^^^

.. java:method:: @Override public void setPoint(int index, Point point)
   :outertype: ArrayFront

sort
^^^^

.. java:method:: @Override public void sort(Comparator<Point> comparator)
   :outertype: ArrayFront

toString
^^^^^^^^

.. java:method:: @Override public String toString()
   :outertype: ArrayFront

