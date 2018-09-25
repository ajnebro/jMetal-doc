.. java:import:: org.apache.commons.lang3.tuple ImmutablePair

.. java:import:: org.apache.commons.lang3.tuple Pair

.. java:import:: org.junit Before

.. java:import:: org.junit Rule

.. java:import:: org.junit Test

.. java:import:: org.junit.rules ExpectedException

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: org.uma.jmetal.util.front Front

.. java:import:: org.uma.jmetal.util.front.imp ArrayFront

.. java:import:: org.uma.jmetal.util.front.util FrontUtils

.. java:import:: org.uma.jmetal.util.point Point

.. java:import:: org.uma.jmetal.util.point.impl ArrayPoint

.. java:import:: java.util ArrayList

.. java:import:: java.util List

SetCoverageTest
===============

.. java:package:: org.uma.jmetal.qualityindicator.impl
   :noindex:

.. java:type:: public class SetCoverageTest

   :author: Antonio J. Nebro

Fields
------
exception
^^^^^^^^^

.. java:field:: @Rule public ExpectedException exception
   :outertype: SetCoverageTest

Methods
-------
setup
^^^^^

.. java:method:: @Before public void setup()
   :outertype: SetCoverageTest

shouldExecuteRaiseAnExceptionIfTheFirstFrontIsNull
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldExecuteRaiseAnExceptionIfTheFirstFrontIsNull()
   :outertype: SetCoverageTest

shouldExecuteRaiseAnExceptionIfTheParetoFrontIsNull
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldExecuteRaiseAnExceptionIfTheParetoFrontIsNull()
   :outertype: SetCoverageTest

shouldExecuteReturnOneIfTheSecondFrontIsEmpty
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldExecuteReturnOneIfTheSecondFrontIsEmpty()
   :outertype: SetCoverageTest

shouldExecuteReturnTheCorrectValueCaseA
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldExecuteReturnTheCorrectValueCaseA()
   :outertype: SetCoverageTest

   Given a frontA with points [0.0,6.0], [2.0,3.0],[4.0,2.0] and a frontB with points [1.0,7.0], [2.0,3.0], [3.5, 1.0], the value of setCoverage(frontA, frontB) == 1/3 and setCoverage(frontB, frontA) == 1/3

shouldExecuteReturnTheCorrectValueCaseB
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldExecuteReturnTheCorrectValueCaseB()
   :outertype: SetCoverageTest

   Given a frontA with points [0.0,6.0], [2.0,3.0],[4.0,2.0] and a frontB with points [1.0,7.0], [2.5,3.0], [5.0, 2.5], the value of setCoverage(frontA, frontB) == 1 and setCoverage(frontB, frontA) == 0

shouldExecuteReturnTheRightValueIfTheFrontsContainOnePointWhichIsNotTheSame
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldExecuteReturnTheRightValueIfTheFrontsContainOnePointWhichIsNotTheSame()
   :outertype: SetCoverageTest

   Given a frontA with point [2,3] and a frontB with point [1,2], the value of the setCoverage(frontA, frontB) == 0 and setCoverage(frontB, frontA) == 1

shouldExecuteReturnZeroIfBothFrontsAreEmpty
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldExecuteReturnZeroIfBothFrontsAreEmpty()
   :outertype: SetCoverageTest

shouldExecuteReturnZeroIfTheFrontsContainOnePointWhichIsTheSame
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldExecuteReturnZeroIfTheFrontsContainOnePointWhichIsTheSame()
   :outertype: SetCoverageTest

shouldGetNameReturnTheCorrectValue
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldGetNameReturnTheCorrectValue()
   :outertype: SetCoverageTest

   The same case as shouldExecuteReturnTheCorrectValueCaseB() but using solution lists

