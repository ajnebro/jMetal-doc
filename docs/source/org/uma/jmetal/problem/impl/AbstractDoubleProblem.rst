.. java:import:: org.uma.jmetal.problem DoubleProblem

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.solution.impl DefaultDoubleSolution

.. java:import:: java.util List

AbstractDoubleProblem
=====================

.. java:package:: org.uma.jmetal.problem.impl
   :noindex:

.. java:type:: @SuppressWarnings public abstract class AbstractDoubleProblem extends AbstractGenericProblem<DoubleSolution> implements DoubleProblem

Methods
-------
createSolution
^^^^^^^^^^^^^^

.. java:method:: @Override public DoubleSolution createSolution()
   :outertype: AbstractDoubleProblem

getLowerBound
^^^^^^^^^^^^^

.. java:method:: @Override public Double getLowerBound(int index)
   :outertype: AbstractDoubleProblem

getUpperBound
^^^^^^^^^^^^^

.. java:method:: @Override public Double getUpperBound(int index)
   :outertype: AbstractDoubleProblem

setLowerLimit
^^^^^^^^^^^^^

.. java:method:: protected void setLowerLimit(List<Double> lowerLimit)
   :outertype: AbstractDoubleProblem

setUpperLimit
^^^^^^^^^^^^^

.. java:method:: protected void setUpperLimit(List<Double> upperLimit)
   :outertype: AbstractDoubleProblem

