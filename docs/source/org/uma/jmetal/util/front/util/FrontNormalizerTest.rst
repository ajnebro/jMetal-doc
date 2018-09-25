.. java:import:: org.junit Rule

.. java:import:: org.junit Test

.. java:import:: org.junit.rules ExpectedException

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: org.uma.jmetal.util.front Front

.. java:import:: org.uma.jmetal.util.front.imp ArrayFront

.. java:import:: org.uma.jmetal.util.point Point

.. java:import:: org.uma.jmetal.util.point.impl ArrayPoint

.. java:import:: org.uma.jmetal.util.point PointSolution

.. java:import:: java.util ArrayList

.. java:import:: java.util Collections

.. java:import:: java.util List

FrontNormalizerTest
===================

.. java:package:: org.uma.jmetal.util.front.util
   :noindex:

.. java:type:: public class FrontNormalizerTest

   :author: Antonio J. Nebro

Fields
------
exception
^^^^^^^^^

.. java:field:: @Rule public ExpectedException exception
   :outertype: FrontNormalizerTest

Methods
-------
shouldFrontNormalizerConstructorRaiseAnExceptionIsTheReferenceFrontIsNull
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldFrontNormalizerConstructorRaiseAnExceptionIsTheReferenceFrontIsNull()
   :outertype: FrontNormalizerTest

shouldFrontNormalizerConstructorRaiseAnExceptionIsTheReferenceSolutionListIsNull
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldFrontNormalizerConstructorRaiseAnExceptionIsTheReferenceSolutionListIsNull()
   :outertype: FrontNormalizerTest

shouldFrontNormalizerConstructorRaiseAnExceptionIsTheVectorOfMaximumValuesIsNull
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldFrontNormalizerConstructorRaiseAnExceptionIsTheVectorOfMaximumValuesIsNull()
   :outertype: FrontNormalizerTest

shouldFrontNormalizerConstructorRaiseAnExceptionIsTheVectorOfMinimumValuesIsNull
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldFrontNormalizerConstructorRaiseAnExceptionIsTheVectorOfMinimumValuesIsNull()
   :outertype: FrontNormalizerTest

shouldFrontNormalizerContructorRaiseAnExceptionTheDimensionOfTheMaximumAndMinimumArrayIsNotEqual
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldFrontNormalizerContructorRaiseAnExceptionTheDimensionOfTheMaximumAndMinimumArrayIsNotEqual()
   :outertype: FrontNormalizerTest

shouldGetNormalizedFrontReturnTheCorrectFrontIfTheSolutionListContainsTwoPoints
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldGetNormalizedFrontReturnTheCorrectFrontIfTheSolutionListContainsTwoPoints()
   :outertype: FrontNormalizerTest

   Points: [2,4], [-2, 3] Maximum values: [6, 8] Minimum values: [-10, 1] Result: [0.5, 1.0], []

shouldGetNormalizedFrontReturnTheCorrectFrontIfThisContainsTwoPoints
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldGetNormalizedFrontReturnTheCorrectFrontIfThisContainsTwoPoints()
   :outertype: FrontNormalizerTest

   Points: [2,4], [-2, 3] Maximum values: [6, 8] Minimum values: [-10, 1] Result: [0.5, 1.0], []

shouldNormalizeRaiseAnExceptionIfTheFrontIsEmpty
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldNormalizeRaiseAnExceptionIfTheFrontIsEmpty()
   :outertype: FrontNormalizerTest

shouldNormalizeRaiseAnExceptionIfTheMaxAndMinValuesAreTheSame
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldNormalizeRaiseAnExceptionIfTheMaxAndMinValuesAreTheSame()
   :outertype: FrontNormalizerTest

   Point: [2,4] Maximum values: [2, 4] Minimum values: [2, 4] Result: [0.5, 1.0]

shouldNormalizeRaiseAnExceptionIfTheSolutionListIsEmpty
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldNormalizeRaiseAnExceptionIfTheSolutionListIsEmpty()
   :outertype: FrontNormalizerTest

shouldNormalizeRaiseAnExceptionTheDimensionOfTheMaximumArrayPointsIsNotCorrect
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldNormalizeRaiseAnExceptionTheDimensionOfTheMaximumArrayPointsIsNotCorrect()
   :outertype: FrontNormalizerTest

shouldNormalizeRaiseAnExceptionTheFrontIsNull
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldNormalizeRaiseAnExceptionTheFrontIsNull()
   :outertype: FrontNormalizerTest

shouldNormalizeRaiseAnExceptionTheSolutionListIsNull
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldNormalizeRaiseAnExceptionTheSolutionListIsNull()
   :outertype: FrontNormalizerTest

shouldNormalizeReturnTheCorrectFrontIfThisContainsOnePoint
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldNormalizeReturnTheCorrectFrontIfThisContainsOnePoint()
   :outertype: FrontNormalizerTest

   Point: [2,4] Maximum values: [4, 4] Minimum values: [0, 0] Result: [0.5, 1.0]

