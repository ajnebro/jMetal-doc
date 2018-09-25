.. java:import:: org.junit After

.. java:import:: org.junit Before

.. java:import:: org.junit Test

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: org.uma.jmetal.util.point Point

.. java:import:: org.uma.jmetal.util.point.util.comparator PointDimensionComparator

PointDimensionComparatorTest
============================

.. java:package:: org.uma.jmetal.util.point.impl
   :noindex:

.. java:type:: public class PointDimensionComparatorTest

   :author: Antonio J. Nebro

Methods
-------
clean
^^^^^

.. java:method:: @After public void clean()
   :outertype: PointDimensionComparatorTest

setup
^^^^^

.. java:method:: @Before public void setup()
   :outertype: PointDimensionComparatorTest

shouldCompareReturnMinusOneIfTheFirstValueIsLower
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldCompareReturnMinusOneIfTheFirstValueIsLower() throws Exception
   :outertype: PointDimensionComparatorTest

shouldCompareReturnPlusOneIfTheFirstValueIsGreater
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldCompareReturnPlusOneIfTheFirstValueIsGreater() throws Exception
   :outertype: PointDimensionComparatorTest

shouldCompareReturnZeroIfTheComparedValuesAreEqual
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldCompareReturnZeroIfTheComparedValuesAreEqual() throws Exception
   :outertype: PointDimensionComparatorTest

shouldFirstPointToCompareEqualsToNullRaiseAnException
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldFirstPointToCompareEqualsToNullRaiseAnException() throws Exception
   :outertype: PointDimensionComparatorTest

shouldIndexLessThanZeroRaiseAnException
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldIndexLessThanZeroRaiseAnException() throws Exception
   :outertype: PointDimensionComparatorTest

shouldIndexValueGreaterThanFirstPointDimensionsRaiseAnException
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldIndexValueGreaterThanFirstPointDimensionsRaiseAnException() throws Exception
   :outertype: PointDimensionComparatorTest

shouldIndexValueGreaterThanSecondPointDimensionsRaiseAnException
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldIndexValueGreaterThanSecondPointDimensionsRaiseAnException() throws Exception
   :outertype: PointDimensionComparatorTest

shouldSecondPointToCompareEqualsToNullRaiseAnException
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldSecondPointToCompareEqualsToNullRaiseAnException() throws Exception
   :outertype: PointDimensionComparatorTest

