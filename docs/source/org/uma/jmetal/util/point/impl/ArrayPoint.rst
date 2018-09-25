.. java:import:: java.io BufferedReader

.. java:import:: java.io FileInputStream

.. java:import:: java.io IOException

.. java:import:: java.io InputStreamReader

.. java:import:: java.util ArrayList

.. java:import:: java.util Arrays

.. java:import:: java.util List

.. java:import:: java.util StringTokenizer

.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: org.uma.jmetal.util.point Point

ArrayPoint
==========

.. java:package:: org.uma.jmetal.util.point.impl
   :noindex:

.. java:type:: public class ArrayPoint implements Point

   Class representing a point (i.e, an array of double values)

   :author: Antonio J. Nebro

Fields
------
point
^^^^^

.. java:field:: protected double[] point
   :outertype: ArrayPoint

Constructors
------------
ArrayPoint
^^^^^^^^^^

.. java:constructor:: public ArrayPoint()
   :outertype: ArrayPoint

   Default constructor

ArrayPoint
^^^^^^^^^^

.. java:constructor:: public ArrayPoint(int dimension)
   :outertype: ArrayPoint

   Constructor

   :param dimension: Dimension of the point

ArrayPoint
^^^^^^^^^^

.. java:constructor:: public ArrayPoint(Point point)
   :outertype: ArrayPoint

   Copy constructor

   :param point:

ArrayPoint
^^^^^^^^^^

.. java:constructor:: public ArrayPoint(double[] point)
   :outertype: ArrayPoint

   Constructor from an array of double values

   :param point:

ArrayPoint
^^^^^^^^^^

.. java:constructor:: public ArrayPoint(String fileName) throws IOException
   :outertype: ArrayPoint

   Constructor reading the values from a file

   :param fileName:

Methods
-------
equals
^^^^^^

.. java:method:: @Override public boolean equals(Object o)
   :outertype: ArrayPoint

getDimension
^^^^^^^^^^^^

.. java:method:: @Override public int getDimension()
   :outertype: ArrayPoint

getValue
^^^^^^^^

.. java:method:: @Override public double getValue(int index)
   :outertype: ArrayPoint

getValues
^^^^^^^^^

.. java:method:: @Override public double[] getValues()
   :outertype: ArrayPoint

hashCode
^^^^^^^^

.. java:method:: @Override public int hashCode()
   :outertype: ArrayPoint

setValue
^^^^^^^^

.. java:method:: @Override public void setValue(int index, double value)
   :outertype: ArrayPoint

toString
^^^^^^^^

.. java:method:: @Override public String toString()
   :outertype: ArrayPoint

update
^^^^^^

.. java:method:: @Override public void update(double[] point)
   :outertype: ArrayPoint

