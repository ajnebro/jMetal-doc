.. java:import:: org.uma.jmetal.problem DoubleBinaryProblem

.. java:import:: org.uma.jmetal.solution DoubleBinarySolution

.. java:import:: java.util BitSet

.. java:import:: java.util HashMap

DefaultDoubleBinarySolution
===========================

.. java:package:: org.uma.jmetal.solution.impl
   :noindex:

.. java:type:: @SuppressWarnings public class DefaultDoubleBinarySolution extends AbstractGenericSolution<Object, DoubleBinaryProblem<?>> implements DoubleBinarySolution

   Description: - this solution contains an array of double value + a binary string - getNumberOfVariables() returns the number of double values + 1 (the string) - getNumberOfDoubleVariables() returns the number of double values - getNumberOfVariables() = getNumberOfDoubleVariables() + 1 - the bitset is the last variable

   :author: Antonio J. Nebro

Constructors
------------
DefaultDoubleBinarySolution
^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public DefaultDoubleBinarySolution(DoubleBinaryProblem<?> problem)
   :outertype: DefaultDoubleBinarySolution

   Constructor

DefaultDoubleBinarySolution
^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public DefaultDoubleBinarySolution(DefaultDoubleBinarySolution solution)
   :outertype: DefaultDoubleBinarySolution

   Copy constructor

Methods
-------
copy
^^^^

.. java:method:: @Override public DefaultDoubleBinarySolution copy()
   :outertype: DefaultDoubleBinarySolution

getLowerBound
^^^^^^^^^^^^^

.. java:method:: @Override public Double getLowerBound(int index)
   :outertype: DefaultDoubleBinarySolution

getNumberOfBits
^^^^^^^^^^^^^^^

.. java:method:: @Override public int getNumberOfBits()
   :outertype: DefaultDoubleBinarySolution

getNumberOfDoubleVariables
^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public int getNumberOfDoubleVariables()
   :outertype: DefaultDoubleBinarySolution

getUpperBound
^^^^^^^^^^^^^

.. java:method:: @Override public Double getUpperBound(int index)
   :outertype: DefaultDoubleBinarySolution

getVariableValueString
^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public String getVariableValueString(int index)
   :outertype: DefaultDoubleBinarySolution

