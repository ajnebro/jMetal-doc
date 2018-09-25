.. java:import:: org.junit Rule

.. java:import:: org.junit Test

.. java:import:: org.junit.rules ExpectedException

.. java:import:: org.uma.jmetal.problem DoubleProblem

.. java:import:: org.uma.jmetal.problem.impl AbstractDoubleProblem

.. java:import:: org.uma.jmetal.qualityindicator QualityIndicator

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: org.uma.jmetal.util.front Front

.. java:import:: org.uma.jmetal.util.front.imp ArrayFront

.. java:import:: org.uma.jmetal.util.front.util FrontUtils

.. java:import:: org.uma.jmetal.util.point Point

.. java:import:: org.uma.jmetal.util.point.impl ArrayPoint

.. java:import:: org.uma.jmetal.util.point PointSolution

.. java:import:: java.io FileNotFoundException

.. java:import:: java.util ArrayList

.. java:import:: java.util Arrays

.. java:import:: java.util List

ErrorRatioTest
==============

.. java:package:: org.uma.jmetal.qualityindicator.impl
   :noindex:

.. java:type:: public class ErrorRatioTest

   :author: Antonio J. Nebro

Fields
------
exception
^^^^^^^^^

.. java:field:: @Rule public ExpectedException exception
   :outertype: ErrorRatioTest

Methods
-------
shouldExecuteRaiseAnExceptionIfTheFrontApproximationIsNull
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldExecuteRaiseAnExceptionIfTheFrontApproximationIsNull()
   :outertype: ErrorRatioTest

shouldExecuteRaiseAnExceptionIfTheParetoFrontApproximationListIsNull
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldExecuteRaiseAnExceptionIfTheParetoFrontApproximationListIsNull()
   :outertype: ErrorRatioTest

shouldExecuteReturnOneIfTheFrontsContainADifferentPoint
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldExecuteReturnOneIfTheFrontsContainADifferentPoint()
   :outertype: ErrorRatioTest

shouldExecuteReturnTheCorrectValueCaseA
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldExecuteReturnTheCorrectValueCaseA()
   :outertype: ErrorRatioTest

   Given a front with points [1.5,4.0], [1.5,2.0],[2.0,1.5] and a Pareto front with points [1.0,3.0], [1.5,2.0], [2.0, 1.5], the value of the epsilon indicator is 2/3

shouldExecuteReturnTheCorrectValueCaseB
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldExecuteReturnTheCorrectValueCaseB()
   :outertype: ErrorRatioTest

   Given a list with solutions [1.5,3.0], [4.0,2.0] and another lists with solutions [-1.0,-1.0], [0.0,0.0], the value of the epsilon indicator is 1

shouldExecuteReturnZeroIfTheFrontsContainOnePointWhichIsTheSame
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldExecuteReturnZeroIfTheFrontsContainOnePointWhichIsTheSame()
   :outertype: ErrorRatioTest

shouldGetNameReturnTheCorrectValue
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldGetNameReturnTheCorrectValue() throws FileNotFoundException
   :outertype: ErrorRatioTest

