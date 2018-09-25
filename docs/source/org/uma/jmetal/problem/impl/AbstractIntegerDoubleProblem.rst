.. java:import:: org.uma.jmetal.problem IntegerDoubleProblem

.. java:import:: java.util List

AbstractIntegerDoubleProblem
============================

.. java:package:: org.uma.jmetal.problem.impl
   :noindex:

.. java:type:: @SuppressWarnings public abstract class AbstractIntegerDoubleProblem<S> extends AbstractGenericProblem<S> implements IntegerDoubleProblem<S>

Methods
-------
getLowerBound
^^^^^^^^^^^^^

.. java:method:: @Override public Number getLowerBound(int index)
   :outertype: AbstractIntegerDoubleProblem

getNumberOfDoubleVariables
^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public int getNumberOfDoubleVariables()
   :outertype: AbstractIntegerDoubleProblem

getNumberOfIntegerVariables
^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public int getNumberOfIntegerVariables()
   :outertype: AbstractIntegerDoubleProblem

getUpperBound
^^^^^^^^^^^^^

.. java:method:: @Override public Number getUpperBound(int index)
   :outertype: AbstractIntegerDoubleProblem

setLowerLimit
^^^^^^^^^^^^^

.. java:method:: protected void setLowerLimit(List<Number> lowerLimit)
   :outertype: AbstractIntegerDoubleProblem

setNumberOfDoubleVariables
^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: protected void setNumberOfDoubleVariables(int numberOfDoubleVariables)
   :outertype: AbstractIntegerDoubleProblem

setNumberOfIntegerVariables
^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: protected void setNumberOfIntegerVariables(int numberOfIntegerVariables)
   :outertype: AbstractIntegerDoubleProblem

setUpperLimit
^^^^^^^^^^^^^

.. java:method:: protected void setUpperLimit(List<Number> upperLimit)
   :outertype: AbstractIntegerDoubleProblem

