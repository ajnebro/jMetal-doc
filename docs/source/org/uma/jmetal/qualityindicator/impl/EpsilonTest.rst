.. java:import:: org.junit Rule

.. java:import:: org.junit Test

.. java:import:: org.junit.rules ExpectedException

.. java:import:: org.uma.jmetal.qualityindicator QualityIndicator

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: org.uma.jmetal.util.front Front

.. java:import:: org.uma.jmetal.util.front.imp ArrayFront

.. java:import:: org.uma.jmetal.util.front.util FrontUtils

.. java:import:: org.uma.jmetal.util.point Point

.. java:import:: org.uma.jmetal.util.point.impl ArrayPoint

.. java:import:: org.uma.jmetal.util.point PointSolution

.. java:import:: java.util List

EpsilonTest
===========

.. java:package:: org.uma.jmetal.qualityindicator.impl
   :noindex:

.. java:type:: public class EpsilonTest

   :author: Antonio J. Nebro

Fields
------
exception
^^^^^^^^^

.. java:field:: @Rule public ExpectedException exception
   :outertype: EpsilonTest

Methods
-------
shouldExecuteRaiseAnExceptionIfTheFrontApproximationIsNull
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldExecuteRaiseAnExceptionIfTheFrontApproximationIsNull()
   :outertype: EpsilonTest

shouldExecuteRaiseAnExceptionIfTheFrontApproximationListIsNull
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldExecuteRaiseAnExceptionIfTheFrontApproximationListIsNull()
   :outertype: EpsilonTest

shouldExecuteReturnTheCorrectValueCaseA
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldExecuteReturnTheCorrectValueCaseA()
   :outertype: EpsilonTest

   Given a front with points [1.5,4.0], [2.0,3.0],[3.0,2.0] and a Pareto front with points [1.0,3.0], [1.5,2.0], [2.0, 1.5], the value of the epsilon indicator is 1

shouldExecuteReturnTheCorrectValueCaseB
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldExecuteReturnTheCorrectValueCaseB()
   :outertype: EpsilonTest

   Given a front with points [1.5,4.0], [1.5,2.0],[2.0,1.5] and a Pareto front with points [1.0,3.0], [1.5,2.0], [2.0, 1.5], the value of the epsilon indicator is 0.5

shouldExecuteReturnTheRightValueIfTheFrontsContainOnePointWhichIsNotTheSame
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldExecuteReturnTheRightValueIfTheFrontsContainOnePointWhichIsNotTheSame()
   :outertype: EpsilonTest

   Given a front with point [2,3] and a Pareto front with point [1,2], the value of the epsilon indicator is 1

shouldExecuteReturnZeroIfTheFrontsContainOnePointWhichIsTheSame
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldExecuteReturnZeroIfTheFrontsContainOnePointWhichIsTheSame()
   :outertype: EpsilonTest

shouldGetNameReturnTheCorrectValue
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldGetNameReturnTheCorrectValue()
   :outertype: EpsilonTest

   The same case as shouldExecuteReturnTheCorrectValueCaseB() but using list of solutions

