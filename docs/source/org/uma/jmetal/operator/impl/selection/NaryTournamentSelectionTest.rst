.. java:import:: org.junit Rule

.. java:import:: org.junit Test

.. java:import:: org.junit.rules ExpectedException

.. java:import:: org.mockito Mockito

.. java:import:: org.springframework.test.util ReflectionTestUtils

.. java:import:: org.uma.jmetal.problem Problem

.. java:import:: org.uma.jmetal.solution BinarySolution

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.solution IntegerSolution

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: java.util ArrayList

.. java:import:: java.util Arrays

.. java:import:: java.util Comparator

.. java:import:: java.util List

NaryTournamentSelectionTest
===========================

.. java:package:: org.uma.jmetal.operator.impl.selection
   :noindex:

.. java:type:: public class NaryTournamentSelectionTest

   :author: Antonio J. Nebro

Fields
------
exception
^^^^^^^^^

.. java:field:: @Rule public ExpectedException exception
   :outertype: NaryTournamentSelectionTest

Methods
-------
shouldDefaultConstructorSetTheNumberOfSolutionsToBeReturnedEqualsToTwo
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldDefaultConstructorSetTheNumberOfSolutionsToBeReturnedEqualsToTwo()
   :outertype: NaryTournamentSelectionTest

shouldExecuteRaiseAnExceptionIfTheListOfSolutionsIsEmpty
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldExecuteRaiseAnExceptionIfTheListOfSolutionsIsEmpty()
   :outertype: NaryTournamentSelectionTest

shouldExecuteRaiseAnExceptionIfTheListOfSolutionsIsNull
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldExecuteRaiseAnExceptionIfTheListOfSolutionsIsNull()
   :outertype: NaryTournamentSelectionTest

shouldExecuteRaiseAnExceptionIfTheListSizeIsOneAndTwoSolutionsAreRequested
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldExecuteRaiseAnExceptionIfTheListSizeIsOneAndTwoSolutionsAreRequested()
   :outertype: NaryTournamentSelectionTest

shouldExecuteReturnAValidSolutionIsWithCorrectParameters
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldExecuteReturnAValidSolutionIsWithCorrectParameters()
   :outertype: NaryTournamentSelectionTest

shouldExecuteReturnTheSameSolutionIfTheListContainsOneSolution
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldExecuteReturnTheSameSolutionIfTheListContainsOneSolution()
   :outertype: NaryTournamentSelectionTest

shouldExecuteReturnTwoSolutionsIfTheListContainsTwoSolutions
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldExecuteReturnTwoSolutionsIfTheListContainsTwoSolutions()
   :outertype: NaryTournamentSelectionTest

