.. java:import:: org.uma.jmetal.problem Problem

.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util.pseudorandom JMetalRandom

AbstractGenericSolution
=======================

.. java:package:: org.uma.jmetal.solution.impl
   :noindex:

.. java:type:: @SuppressWarnings public abstract class AbstractGenericSolution<T, P extends Problem<?>> implements Solution<T>

   Abstract class representing a generic solution

   :author: Antonio J. Nebro

Fields
------
attributes
^^^^^^^^^^

.. java:field:: protected Map<Object, Object> attributes
   :outertype: AbstractGenericSolution

problem
^^^^^^^

.. java:field:: protected P problem
   :outertype: AbstractGenericSolution

randomGenerator
^^^^^^^^^^^^^^^

.. java:field:: protected final JMetalRandom randomGenerator
   :outertype: AbstractGenericSolution

Constructors
------------
AbstractGenericSolution
^^^^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: protected AbstractGenericSolution(P problem)
   :outertype: AbstractGenericSolution

   Constructor

Methods
-------
equals
^^^^^^

.. java:method:: @Override public boolean equals(Object o)
   :outertype: AbstractGenericSolution

getAttribute
^^^^^^^^^^^^

.. java:method:: @Override public Object getAttribute(Object id)
   :outertype: AbstractGenericSolution

getNumberOfObjectives
^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public int getNumberOfObjectives()
   :outertype: AbstractGenericSolution

getNumberOfVariables
^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public int getNumberOfVariables()
   :outertype: AbstractGenericSolution

getObjective
^^^^^^^^^^^^

.. java:method:: @Override public double getObjective(int index)
   :outertype: AbstractGenericSolution

getObjectives
^^^^^^^^^^^^^

.. java:method:: @Override public double[] getObjectives()
   :outertype: AbstractGenericSolution

getVariableValue
^^^^^^^^^^^^^^^^

.. java:method:: @Override public T getVariableValue(int index)
   :outertype: AbstractGenericSolution

hashCode
^^^^^^^^

.. java:method:: @Override public int hashCode()
   :outertype: AbstractGenericSolution

initializeObjectiveValues
^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: protected void initializeObjectiveValues()
   :outertype: AbstractGenericSolution

setAttribute
^^^^^^^^^^^^

.. java:method:: @Override public void setAttribute(Object id, Object value)
   :outertype: AbstractGenericSolution

setObjective
^^^^^^^^^^^^

.. java:method:: @Override public void setObjective(int index, double value)
   :outertype: AbstractGenericSolution

setVariableValue
^^^^^^^^^^^^^^^^

.. java:method:: @Override public void setVariableValue(int index, T value)
   :outertype: AbstractGenericSolution

toString
^^^^^^^^

.. java:method:: @Override public String toString()
   :outertype: AbstractGenericSolution

