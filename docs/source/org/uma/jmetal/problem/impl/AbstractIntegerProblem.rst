.. java:import:: org.uma.jmetal.problem IntegerProblem

.. java:import:: org.uma.jmetal.solution IntegerSolution

.. java:import:: org.uma.jmetal.solution.impl DefaultIntegerSolution

.. java:import:: java.util List

AbstractIntegerProblem
======================

.. java:package:: org.uma.jmetal.problem.impl
   :noindex:

.. java:type:: @SuppressWarnings public abstract class AbstractIntegerProblem extends AbstractGenericProblem<IntegerSolution> implements IntegerProblem

Methods
-------
createSolution
^^^^^^^^^^^^^^

.. java:method:: @Override public IntegerSolution createSolution()
   :outertype: AbstractIntegerProblem

getLowerBound
^^^^^^^^^^^^^

.. java:method:: @Override public Integer getLowerBound(int index)
   :outertype: AbstractIntegerProblem

getUpperBound
^^^^^^^^^^^^^

.. java:method:: @Override public Integer getUpperBound(int index)
   :outertype: AbstractIntegerProblem

setLowerLimit
^^^^^^^^^^^^^

.. java:method:: protected void setLowerLimit(List<Integer> lowerLimit)
   :outertype: AbstractIntegerProblem

setUpperLimit
^^^^^^^^^^^^^

.. java:method:: protected void setUpperLimit(List<Integer> upperLimit)
   :outertype: AbstractIntegerProblem

