.. java:import:: org.uma.jmetal.problem DoubleProblem

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: java.util HashMap

DefaultDoubleSolution
=====================

.. java:package:: org.uma.jmetal.solution.impl
   :noindex:

.. java:type:: @SuppressWarnings public class DefaultDoubleSolution extends AbstractGenericSolution<Double, DoubleProblem> implements DoubleSolution

   Defines an implementation of a double solution

   :author: Antonio J. Nebro

Constructors
------------
DefaultDoubleSolution
^^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public DefaultDoubleSolution(DoubleProblem problem)
   :outertype: DefaultDoubleSolution

   Constructor

DefaultDoubleSolution
^^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public DefaultDoubleSolution(DefaultDoubleSolution solution)
   :outertype: DefaultDoubleSolution

   Copy constructor

Methods
-------
copy
^^^^

.. java:method:: @Override public DefaultDoubleSolution copy()
   :outertype: DefaultDoubleSolution

getLowerBound
^^^^^^^^^^^^^

.. java:method:: @Override public Double getLowerBound(int index)
   :outertype: DefaultDoubleSolution

getUpperBound
^^^^^^^^^^^^^

.. java:method:: @Override public Double getUpperBound(int index)
   :outertype: DefaultDoubleSolution

getVariableValueString
^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public String getVariableValueString(int index)
   :outertype: DefaultDoubleSolution

