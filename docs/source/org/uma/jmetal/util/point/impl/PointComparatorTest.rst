.. java:import:: org.junit Test

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: org.uma.jmetal.util.point Point

.. java:import:: org.uma.jmetal.util.point.util.comparator PointComparator

PointComparatorTest
===================

.. java:package:: org.uma.jmetal.util.point.impl
   :noindex:

.. java:type:: public class PointComparatorTest

   :author: Antonio J. Nebro

Methods
-------
shouldCompareBetterReturnZeroIfBothPointsAreEqualWhenMaximizing
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldCompareBetterReturnZeroIfBothPointsAreEqualWhenMaximizing()
   :outertype: PointComparatorTest

shouldCompareBetterReturnZeroIfBothPointsAreEqualWhenMinimizing
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldCompareBetterReturnZeroIfBothPointsAreEqualWhenMinimizing()
   :outertype: PointComparatorTest

shouldCompareReturnMinusOneIfTheFirstPointIsBetterThanTheSecondOneWhenMaximizing
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldCompareReturnMinusOneIfTheFirstPointIsBetterThanTheSecondOneWhenMaximizing()
   :outertype: PointComparatorTest

shouldCompareReturnOneIfTheSecondPointIsBetterThanTheFirstOneWhenMaximizing
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldCompareReturnOneIfTheSecondPointIsBetterThanTheFirstOneWhenMaximizing()
   :outertype: PointComparatorTest

shouldComparingDifferentLengthPointsRaiseAnException
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldComparingDifferentLengthPointsRaiseAnException() throws Exception
   :outertype: PointComparatorTest

shouldFirstPointToCompareEqualsToNullRaiseAnException
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldFirstPointToCompareEqualsToNullRaiseAnException() throws Exception
   :outertype: PointComparatorTest

shouldSecondPointToCompareEqualsToNullRaiseAnException
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldSecondPointToCompareEqualsToNullRaiseAnException() throws Exception
   :outertype: PointComparatorTest

