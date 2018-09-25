.. java:import:: org.junit Rule

.. java:import:: org.junit Test

.. java:import:: org.junit.rules ExpectedException

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: org.uma.jmetal.util.front Front

.. java:import:: org.uma.jmetal.util.front.util FrontUtils

.. java:import:: org.uma.jmetal.util.point Point

.. java:import:: org.uma.jmetal.util.point.impl ArrayPoint

.. java:import:: org.uma.jmetal.util.point PointSolution

.. java:import:: java.util List

FrontUtilsTest
==============

.. java:package:: org.uma.jmetal.util.front.imp
   :noindex:

.. java:type:: public class FrontUtilsTest

   :author: Antonio J. Nebro

Fields
------
exception
^^^^^^^^^

.. java:field:: @Rule public ExpectedException exception
   :outertype: FrontUtilsTest

Methods
-------
shouldConvertFrontToArrayRaiseAnExceptionIfTheFrontIsNull
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldConvertFrontToArrayRaiseAnExceptionIfTheFrontIsNull()
   :outertype: FrontUtilsTest

shouldConvertFrontToArrayReturnAnEmptyArrayIfTheFrontIsEmpty
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldConvertFrontToArrayReturnAnEmptyArrayIfTheFrontIsEmpty()
   :outertype: FrontUtilsTest

shouldConvertFrontToArrayReturnTheCorrectArrayCaseA
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldConvertFrontToArrayReturnTheCorrectArrayCaseA()
   :outertype: FrontUtilsTest

   Case A: The front has one point

shouldConvertFrontToArrayReturnTheCorrectArrayCaseB
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldConvertFrontToArrayReturnTheCorrectArrayCaseB()
   :outertype: FrontUtilsTest

   Case A: The front has one three points

shouldConvertFrontToSolutionListRaiseAnExceptionIfTheFrontIsNull
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldConvertFrontToSolutionListRaiseAnExceptionIfTheFrontIsNull()
   :outertype: FrontUtilsTest

shouldConvertFrontToSolutionListReturnAnEmptyListIfTheFrontIsEmpty
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldConvertFrontToSolutionListReturnAnEmptyListIfTheFrontIsEmpty()
   :outertype: FrontUtilsTest

shouldConvertFrontToSolutionListReturnTheCorrectListCaseA
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldConvertFrontToSolutionListReturnTheCorrectListCaseA()
   :outertype: FrontUtilsTest

   Case A: The front has one point

shouldConvertFrontToSolutionListReturnTheCorrectListCaseB
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldConvertFrontToSolutionListReturnTheCorrectListCaseB()
   :outertype: FrontUtilsTest

   Case A: The front has one three points

shouldDistanceToClosestPointRaiseAnExceptionIfTheFrontIsEmpty
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldDistanceToClosestPointRaiseAnExceptionIfTheFrontIsEmpty()
   :outertype: FrontUtilsTest

shouldDistanceToClosestPointRaiseAnExceptionIfTheFrontIsNull
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldDistanceToClosestPointRaiseAnExceptionIfTheFrontIsNull()
   :outertype: FrontUtilsTest

shouldDistanceToClosestPointRaiseAnExceptionIfThePointIsNull
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldDistanceToClosestPointRaiseAnExceptionIfThePointIsNull()
   :outertype: FrontUtilsTest

shouldDistanceToClosestPointReturnMaxZeroIfThePointIsTheOnlyPointInTheFront
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldDistanceToClosestPointReturnMaxZeroIfThePointIsTheOnlyPointInTheFront()
   :outertype: FrontUtilsTest

shouldDistanceToClosestPointReturnTheCorrectValueIfTheFrontHasHasOnePoint
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldDistanceToClosestPointReturnTheCorrectValueIfTheFrontHasHasOnePoint()
   :outertype: FrontUtilsTest

shouldDistanceToNearestPointClosestTheCorrectValueIfTheFrontHasTwoPointsCaseA
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldDistanceToNearestPointClosestTheCorrectValueIfTheFrontHasTwoPointsCaseA()
   :outertype: FrontUtilsTest

   Case A: the front has two points and one of them is the point passed as a parameter

shouldDistanceToNearestPointClosestTheCorrectValueIfTheFrontHasTwoPointsCaseB
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldDistanceToNearestPointClosestTheCorrectValueIfTheFrontHasTwoPointsCaseB()
   :outertype: FrontUtilsTest

   Case B: the front has two points and none of them is the point passed as a parameter. The dimensions of the points are ordered

shouldDistanceToNearestPointClosestTheCorrectValueIfTheFrontHasTwoPointsCaseC
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldDistanceToNearestPointClosestTheCorrectValueIfTheFrontHasTwoPointsCaseC()
   :outertype: FrontUtilsTest

   Case B: the front has two points and none of them is the point passed as a parameter. The dimensions of the points are not ordered

shouldDistanceToNearestPointRaiseAnExceptionIfTheFrontIsEmpty
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldDistanceToNearestPointRaiseAnExceptionIfTheFrontIsEmpty()
   :outertype: FrontUtilsTest

shouldDistanceToNearestPointRaiseAnExceptionIfTheFrontIsNull
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldDistanceToNearestPointRaiseAnExceptionIfTheFrontIsNull()
   :outertype: FrontUtilsTest

shouldDistanceToNearestPointRaiseAnExceptionIfThePointIsNull
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldDistanceToNearestPointRaiseAnExceptionIfThePointIsNull()
   :outertype: FrontUtilsTest

shouldDistanceToNearestPointReturnMaxDoubleIfThePointIsTheOnlyPointInTheFront
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldDistanceToNearestPointReturnMaxDoubleIfThePointIsTheOnlyPointInTheFront()
   :outertype: FrontUtilsTest

shouldDistanceToNearestPointReturnTheCorrectValueIfTheFrontHasHasOnePoint
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldDistanceToNearestPointReturnTheCorrectValueIfTheFrontHasHasOnePoint()
   :outertype: FrontUtilsTest

shouldDistanceToNearestPointReturnTheCorrectValueIfTheFrontHasTwoPointsCaseA
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldDistanceToNearestPointReturnTheCorrectValueIfTheFrontHasTwoPointsCaseA()
   :outertype: FrontUtilsTest

   Case A: the front has two points and one of them is the point passed as a parameter

shouldGetInvertedFrontRaiseAnExceptionIfTheFrontIsEmpty
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldGetInvertedFrontRaiseAnExceptionIfTheFrontIsEmpty()
   :outertype: FrontUtilsTest

shouldGetInvertedFrontRaiseAnExceptionIfTheFrontIsNull
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldGetInvertedFrontRaiseAnExceptionIfTheFrontIsNull()
   :outertype: FrontUtilsTest

shouldGetInvertedFrontReturnTheCorrectFrontIfItComposedOfFourPoints
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldGetInvertedFrontReturnTheCorrectFrontIfItComposedOfFourPoints()
   :outertype: FrontUtilsTest

   The front has the points [0.1, 0.9], [0.2, 0.8], [0.3, 0.7], [0.4, 0.6]. The inverted front is [0.9, 0.1], [0.8, 0.2], [0.7, 0.3], [0.6, 0.4]

shouldGetInvertedFrontReturnTheCorrectFrontIfItComposedOfOnePointCaseA
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldGetInvertedFrontReturnTheCorrectFrontIfItComposedOfOnePointCaseA()
   :outertype: FrontUtilsTest

   Case A: the front has the point [0.5, 0.5]. The inverted front is the same

shouldGetInvertedFrontReturnTheCorrectFrontIfItComposedOfOnePointCaseB
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldGetInvertedFrontReturnTheCorrectFrontIfItComposedOfOnePointCaseB()
   :outertype: FrontUtilsTest

   Case B: the front has the point [0.0, 1.0]. The inverted front is [1.0, 0.0]

shouldGetInvertedFrontReturnTheCorrectFrontIfItComposedOfOnePointCaseC
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldGetInvertedFrontReturnTheCorrectFrontIfItComposedOfOnePointCaseC()
   :outertype: FrontUtilsTest

   Case C: the front has the point [3.0, -2.0]. The inverted front is [0.0, 1.0]

shouldGetMaximumValuesRaiseAnExceptionIfTheFrontIsEmpty
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldGetMaximumValuesRaiseAnExceptionIfTheFrontIsEmpty()
   :outertype: FrontUtilsTest

shouldGetMaximumValuesRaiseAnExceptionIfTheFrontIsNull
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldGetMaximumValuesRaiseAnExceptionIfTheFrontIsNull()
   :outertype: FrontUtilsTest

shouldGetMaximumValuesWithAFrontWithOnePointReturnTheCorrectValue
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldGetMaximumValuesWithAFrontWithOnePointReturnTheCorrectValue()
   :outertype: FrontUtilsTest

shouldGetMaximumValuesWithAFrontWithThreePointReturnTheCorrectValue
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldGetMaximumValuesWithAFrontWithThreePointReturnTheCorrectValue()
   :outertype: FrontUtilsTest

shouldGetMinimumValuesRaiseAnExceptionIfTheFrontIsEmpty
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldGetMinimumValuesRaiseAnExceptionIfTheFrontIsEmpty()
   :outertype: FrontUtilsTest

shouldGetMinimumValuesRaiseAnExceptionIfTheFrontIsNull
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldGetMinimumValuesRaiseAnExceptionIfTheFrontIsNull()
   :outertype: FrontUtilsTest

shouldGetMinimumValuesWithAFrontWithOnePointReturnTheCorrectValue
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldGetMinimumValuesWithAFrontWithOnePointReturnTheCorrectValue()
   :outertype: FrontUtilsTest

shouldGetMinimumValuesWithAFrontWithThreePointReturnTheCorrectValue
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldGetMinimumValuesWithAFrontWithThreePointReturnTheCorrectValue()
   :outertype: FrontUtilsTest

