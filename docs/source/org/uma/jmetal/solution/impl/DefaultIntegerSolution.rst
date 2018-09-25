.. java:import:: org.uma.jmetal.problem IntegerProblem

.. java:import:: org.uma.jmetal.solution IntegerSolution

.. java:import:: java.util HashMap

DefaultIntegerSolution
======================

.. java:package:: org.uma.jmetal.solution.impl
   :noindex:

.. java:type:: @SuppressWarnings public class DefaultIntegerSolution extends AbstractGenericSolution<Integer, IntegerProblem> implements IntegerSolution

   Defines an implementation of an integer solution

   :author: Antonio J. Nebro

Constructors
------------
DefaultIntegerSolution
^^^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public DefaultIntegerSolution(IntegerProblem problem)
   :outertype: DefaultIntegerSolution

   Constructor

DefaultIntegerSolution
^^^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public DefaultIntegerSolution(DefaultIntegerSolution solution)
   :outertype: DefaultIntegerSolution

   Copy constructor

Methods
-------
copy
^^^^

.. java:method:: @Override public DefaultIntegerSolution copy()
   :outertype: DefaultIntegerSolution

getLowerBound
^^^^^^^^^^^^^

.. java:method:: @Override public Integer getLowerBound(int index)
   :outertype: DefaultIntegerSolution

getUpperBound
^^^^^^^^^^^^^

.. java:method:: @Override public Integer getUpperBound(int index)
   :outertype: DefaultIntegerSolution

getVariableValueString
^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public String getVariableValueString(int index)
   :outertype: DefaultIntegerSolution

