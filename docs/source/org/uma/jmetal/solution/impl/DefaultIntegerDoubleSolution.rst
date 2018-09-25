.. java:import:: org.uma.jmetal.problem IntegerDoubleProblem

.. java:import:: org.uma.jmetal.solution IntegerDoubleSolution

.. java:import:: java.util HashMap

DefaultIntegerDoubleSolution
============================

.. java:package:: org.uma.jmetal.solution.impl
   :noindex:

.. java:type:: @SuppressWarnings public class DefaultIntegerDoubleSolution extends AbstractGenericSolution<Number, IntegerDoubleProblem<?>> implements IntegerDoubleSolution

   Defines an implementation of a class for solutions having integers and doubles

   :author: Antonio J. Nebro

Constructors
------------
DefaultIntegerDoubleSolution
^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public DefaultIntegerDoubleSolution(IntegerDoubleProblem<?> problem)
   :outertype: DefaultIntegerDoubleSolution

   Constructor

DefaultIntegerDoubleSolution
^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public DefaultIntegerDoubleSolution(DefaultIntegerDoubleSolution solution)
   :outertype: DefaultIntegerDoubleSolution

   Copy constructor

Methods
-------
copy
^^^^

.. java:method:: @Override public DefaultIntegerDoubleSolution copy()
   :outertype: DefaultIntegerDoubleSolution

getLowerBound
^^^^^^^^^^^^^

.. java:method:: @Override public Number getLowerBound(int index)
   :outertype: DefaultIntegerDoubleSolution

getNumberOfDoubleVariables
^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public int getNumberOfDoubleVariables()
   :outertype: DefaultIntegerDoubleSolution

getNumberOfIntegerVariables
^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public int getNumberOfIntegerVariables()
   :outertype: DefaultIntegerDoubleSolution

getUpperBound
^^^^^^^^^^^^^

.. java:method:: @Override public Number getUpperBound(int index)
   :outertype: DefaultIntegerDoubleSolution

getVariableValueString
^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public String getVariableValueString(int index)
   :outertype: DefaultIntegerDoubleSolution

