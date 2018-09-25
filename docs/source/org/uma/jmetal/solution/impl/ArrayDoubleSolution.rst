.. java:import:: org.uma.jmetal.problem DoubleProblem

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util.pseudorandom JMetalRandom

.. java:import:: java.util Arrays

.. java:import:: java.util HashMap

.. java:import:: java.util Map

ArrayDoubleSolution
===================

.. java:package:: org.uma.jmetal.solution.impl
   :noindex:

.. java:type:: @SuppressWarnings public class ArrayDoubleSolution implements DoubleSolution

   Implementation of \ :java:ref:`DoubleSolution`\  using arrays.

   :author: Antonio J. Nebro

Fields
------
attributes
^^^^^^^^^^

.. java:field:: protected Map<Object, Object> attributes
   :outertype: ArrayDoubleSolution

problem
^^^^^^^

.. java:field:: protected DoubleProblem problem
   :outertype: ArrayDoubleSolution

randomGenerator
^^^^^^^^^^^^^^^

.. java:field:: protected final JMetalRandom randomGenerator
   :outertype: ArrayDoubleSolution

Constructors
------------
ArrayDoubleSolution
^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public ArrayDoubleSolution(DoubleProblem problem)
   :outertype: ArrayDoubleSolution

   Constructor

ArrayDoubleSolution
^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public ArrayDoubleSolution(ArrayDoubleSolution solution)
   :outertype: ArrayDoubleSolution

   Copy constructor

   :param solution: to copy

Methods
-------
copy
^^^^

.. java:method:: @Override public Solution<Double> copy()
   :outertype: ArrayDoubleSolution

equals
^^^^^^

.. java:method:: @Override public boolean equals(Object o)
   :outertype: ArrayDoubleSolution

getAttribute
^^^^^^^^^^^^

.. java:method:: @Override public Object getAttribute(Object id)
   :outertype: ArrayDoubleSolution

getLowerBound
^^^^^^^^^^^^^

.. java:method:: @Override public Double getLowerBound(int index)
   :outertype: ArrayDoubleSolution

getNumberOfObjectives
^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public int getNumberOfObjectives()
   :outertype: ArrayDoubleSolution

getNumberOfVariables
^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public int getNumberOfVariables()
   :outertype: ArrayDoubleSolution

getObjective
^^^^^^^^^^^^

.. java:method:: @Override public double getObjective(int index)
   :outertype: ArrayDoubleSolution

getObjectives
^^^^^^^^^^^^^

.. java:method:: @Override public double[] getObjectives()
   :outertype: ArrayDoubleSolution

getUpperBound
^^^^^^^^^^^^^

.. java:method:: @Override public Double getUpperBound(int index)
   :outertype: ArrayDoubleSolution

getVariableValue
^^^^^^^^^^^^^^^^

.. java:method:: @Override public Double getVariableValue(int index)
   :outertype: ArrayDoubleSolution

getVariableValueString
^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public String getVariableValueString(int index)
   :outertype: ArrayDoubleSolution

hashCode
^^^^^^^^

.. java:method:: @Override public int hashCode()
   :outertype: ArrayDoubleSolution

setAttribute
^^^^^^^^^^^^

.. java:method:: @Override public void setAttribute(Object id, Object value)
   :outertype: ArrayDoubleSolution

setObjective
^^^^^^^^^^^^

.. java:method:: @Override public void setObjective(int index, double value)
   :outertype: ArrayDoubleSolution

setVariableValue
^^^^^^^^^^^^^^^^

.. java:method:: @Override public void setVariableValue(int index, Double value)
   :outertype: ArrayDoubleSolution

