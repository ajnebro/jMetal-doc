.. java:import:: org.junit Rule

.. java:import:: org.junit Test

.. java:import:: org.junit.rules ExpectedException

.. java:import:: org.springframework.test.util ReflectionTestUtils

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: java.util ArrayList

.. java:import:: java.util List

RankingAndCrowdingSelectionTest
===============================

.. java:package:: org.uma.jmetal.operator.impl.selection
   :noindex:

.. java:type:: public class RankingAndCrowdingSelectionTest

   :author: Antonio J. Nebro

Fields
------
exception
^^^^^^^^^

.. java:field:: @Rule public ExpectedException exception
   :outertype: RankingAndCrowdingSelectionTest

Methods
-------
shouldDefaultConstructorReturnASingleSolution
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldDefaultConstructorReturnASingleSolution()
   :outertype: RankingAndCrowdingSelectionTest

shouldExecuteRaiseAnExceptionIfTheSolutionListIsEmpty
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldExecuteRaiseAnExceptionIfTheSolutionListIsEmpty()
   :outertype: RankingAndCrowdingSelectionTest

shouldExecuteRaiseAnExceptionIfTheSolutionListIsNull
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldExecuteRaiseAnExceptionIfTheSolutionListIsNull()
   :outertype: RankingAndCrowdingSelectionTest

shouldNonDefaultConstructorReturnTheCorrectNumberOfSolutions
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldNonDefaultConstructorReturnTheCorrectNumberOfSolutions()
   :outertype: RankingAndCrowdingSelectionTest

