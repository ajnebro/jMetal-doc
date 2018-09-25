.. java:import:: java.util Arrays

.. java:import:: java.util HashMap

.. java:import:: java.util Map

.. java:import:: org.uma.jmetal.solution Solution

PointSolution
=============

.. java:package:: org.uma.jmetal.util.point
   :noindex:

.. java:type:: @SuppressWarnings public class PointSolution implements Solution<Double>

   Solution used to wrap a \ :java:ref:`Point`\  object. Only objectives are used.

   :author: Antonio J. Nebro

Fields
------
attributes
^^^^^^^^^^

.. java:field:: protected Map<Object, Object> attributes
   :outertype: PointSolution

Constructors
------------
PointSolution
^^^^^^^^^^^^^

.. java:constructor:: public PointSolution(int numberOfObjectives)
   :outertype: PointSolution

   Constructor

   :param numberOfObjectives:

PointSolution
^^^^^^^^^^^^^

.. java:constructor:: public PointSolution(Point point)
   :outertype: PointSolution

   Constructor

   :param point:

PointSolution
^^^^^^^^^^^^^

.. java:constructor:: public PointSolution(Solution<?> solution)
   :outertype: PointSolution

   Constructor

   :param solution:

PointSolution
^^^^^^^^^^^^^

.. java:constructor:: public PointSolution(PointSolution point)
   :outertype: PointSolution

   Copy constructor

   :param point:

Methods
-------
copy
^^^^

.. java:method:: @Override public PointSolution copy()
   :outertype: PointSolution

equals
^^^^^^

.. java:method:: @Override public boolean equals(Object o)
   :outertype: PointSolution

getAttribute
^^^^^^^^^^^^

.. java:method:: @Override public Object getAttribute(Object id)
   :outertype: PointSolution

getNumberOfObjectives
^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public int getNumberOfObjectives()
   :outertype: PointSolution

getNumberOfVariables
^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public int getNumberOfVariables()
   :outertype: PointSolution

getObjective
^^^^^^^^^^^^

.. java:method:: @Override public double getObjective(int index)
   :outertype: PointSolution

getObjectives
^^^^^^^^^^^^^

.. java:method:: @Override public double[] getObjectives()
   :outertype: PointSolution

getVariableValue
^^^^^^^^^^^^^^^^

.. java:method:: @Override public Double getVariableValue(int index)
   :outertype: PointSolution

getVariableValueString
^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public String getVariableValueString(int index)
   :outertype: PointSolution

hashCode
^^^^^^^^

.. java:method:: @Override public int hashCode()
   :outertype: PointSolution

setAttribute
^^^^^^^^^^^^

.. java:method:: @Override public void setAttribute(Object id, Object value)
   :outertype: PointSolution

setObjective
^^^^^^^^^^^^

.. java:method:: @Override public void setObjective(int index, double value)
   :outertype: PointSolution

setVariableValue
^^^^^^^^^^^^^^^^

.. java:method:: @Override public void setVariableValue(int index, Double value)
   :outertype: PointSolution

toString
^^^^^^^^

.. java:method:: @Override public String toString()
   :outertype: PointSolution

