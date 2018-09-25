.. java:import:: org.junit Rule

.. java:import:: org.junit Test

.. java:import:: org.junit.rules ExpectedException

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: org.uma.jmetal.util.front Front

.. java:import:: org.uma.jmetal.util.front.imp ArrayFront

.. java:import:: org.uma.jmetal.util.front.util FrontUtils

.. java:import:: org.uma.jmetal.util.point Point

.. java:import:: org.uma.jmetal.util.point.impl ArrayPoint

.. java:import:: org.uma.jmetal.util.point PointSolution

.. java:import:: java.io FileNotFoundException

InvertedGenerationalDistancePlusTest
====================================

.. java:package:: org.uma.jmetal.qualityindicator.impl
   :noindex:

.. java:type:: public class InvertedGenerationalDistancePlusTest

   :author: Antonio J. Nebro

Fields
------
exception
^^^^^^^^^

.. java:field:: @Rule public ExpectedException exception
   :outertype: InvertedGenerationalDistancePlusTest

Methods
-------
shouldConstructorRaiseAnExceptionIfFileNameIsNull
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldConstructorRaiseAnExceptionIfFileNameIsNull() throws FileNotFoundException
   :outertype: InvertedGenerationalDistancePlusTest

shouldConstructorRaiseAnExceptionIfTheParetoFrontIsNull
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldConstructorRaiseAnExceptionIfTheParetoFrontIsNull()
   :outertype: InvertedGenerationalDistancePlusTest

shouldEvaluateRaiseAnExceptionIfTheFrontApproximationIsNull
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldEvaluateRaiseAnExceptionIfTheFrontApproximationIsNull()
   :outertype: InvertedGenerationalDistancePlusTest

shouldEvaluateReturnTheCorrectValueCaseA
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldEvaluateReturnTheCorrectValueCaseA()
   :outertype: InvertedGenerationalDistancePlusTest

shouldEvaluateReturnTheCorrectValueCaseB
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldEvaluateReturnTheCorrectValueCaseB()
   :outertype: InvertedGenerationalDistancePlusTest

shouldEvaluateReturnZeroIfTheFrontAndTheReferenceFrontContainsTheSamePoints
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldEvaluateReturnZeroIfTheFrontAndTheReferenceFrontContainsTheSamePoints()
   :outertype: InvertedGenerationalDistancePlusTest

