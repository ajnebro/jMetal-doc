.. java:import:: java.io Serializable

Solution
========

.. java:package:: org.uma.jmetal.solution
   :noindex:

.. java:type:: public interface Solution<T> extends Serializable

   Interface representing a Solution

   :author: Antonio J. Nebro
   :param <T>: Type (Double, Integer, etc.)

Methods
-------
copy
^^^^

.. java:method::  Solution<T> copy()
   :outertype: Solution

getAttribute
^^^^^^^^^^^^

.. java:method::  Object getAttribute(Object id)
   :outertype: Solution

getNumberOfObjectives
^^^^^^^^^^^^^^^^^^^^^

.. java:method::  int getNumberOfObjectives()
   :outertype: Solution

getNumberOfVariables
^^^^^^^^^^^^^^^^^^^^

.. java:method::  int getNumberOfVariables()
   :outertype: Solution

getObjective
^^^^^^^^^^^^

.. java:method::  double getObjective(int index)
   :outertype: Solution

getObjectives
^^^^^^^^^^^^^

.. java:method::  double[] getObjectives()
   :outertype: Solution

getVariableValue
^^^^^^^^^^^^^^^^

.. java:method::  T getVariableValue(int index)
   :outertype: Solution

getVariableValueString
^^^^^^^^^^^^^^^^^^^^^^

.. java:method::  String getVariableValueString(int index)
   :outertype: Solution

setAttribute
^^^^^^^^^^^^

.. java:method::  void setAttribute(Object id, Object value)
   :outertype: Solution

setObjective
^^^^^^^^^^^^

.. java:method::  void setObjective(int index, double value)
   :outertype: Solution

setVariableValue
^^^^^^^^^^^^^^^^

.. java:method::  void setVariableValue(int index, T value)
   :outertype: Solution

