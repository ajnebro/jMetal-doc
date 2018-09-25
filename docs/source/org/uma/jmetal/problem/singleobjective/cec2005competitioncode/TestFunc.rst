.. java:import:: org.uma.jmetal.util JMetalException

TestFunc
========

.. java:package:: org.uma.jmetal.problem.singleobjective.cec2005competitioncode
   :noindex:

.. java:type:: public abstract class TestFunc

Fields
------
mBias
^^^^^

.. java:field:: protected double mBias
   :outertype: TestFunc

mDimension
^^^^^^^^^^

.. java:field:: protected int mDimension
   :outertype: TestFunc

mFuncName
^^^^^^^^^

.. java:field:: protected String mFuncName
   :outertype: TestFunc

Constructors
------------
TestFunc
^^^^^^^^

.. java:constructor:: public TestFunc(int dimension, double bias)
   :outertype: TestFunc

TestFunc
^^^^^^^^

.. java:constructor:: public TestFunc(int dimension, double bias, String funcName)
   :outertype: TestFunc

Methods
-------
bias
^^^^

.. java:method:: public double bias()
   :outertype: TestFunc

dimension
^^^^^^^^^

.. java:method:: public int dimension()
   :outertype: TestFunc

f
^

.. java:method:: public abstract double f(double[] x) throws JMetalException
   :outertype: TestFunc

name
^^^^

.. java:method:: public String name()
   :outertype: TestFunc

