.. java:import:: org.junit Rule

.. java:import:: org.junit Test

.. java:import:: org.junit.rules ExpectedException

.. java:import:: org.mockito Matchers

.. java:import:: org.uma.jmetal.problem Problem

.. java:import:: org.uma.jmetal.problem.impl AbstractDoubleProblem

.. java:import:: org.uma.jmetal.solution BinarySolution

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.solution IntegerSolution

.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util.pseudorandom JMetalRandom

.. java:import:: org.uma.jmetal.util.pseudorandom.impl AuditableRandomGenerator

SolutionListUtilsTest
=====================

.. java:package:: org.uma.jmetal.util
   :noindex:

.. java:type:: public class SolutionListUtilsTest

   :author: Antonio J. Nebro

Fields
------
exception
^^^^^^^^^

.. java:field:: @Rule public ExpectedException exception
   :outertype: SolutionListUtilsTest

Methods
-------
shouldExecuteReturnTheSolutionInTheListIfTheListContainsASolution
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldExecuteReturnTheSolutionInTheListIfTheListContainsASolution()
   :outertype: SolutionListUtilsTest

shouldFillPopulationWithNewSolutionsDoNothingIfTheMaxSizeIsLowerThanTheListSize
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldFillPopulationWithNewSolutionsDoNothingIfTheMaxSizeIsLowerThanTheListSize()
   :outertype: SolutionListUtilsTest

shouldFillPopulationWithNewSolutionsIncreaseTheListLengthToTheIndicatedValue
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldFillPopulationWithNewSolutionsIncreaseTheListLengthToTheIndicatedValue()
   :outertype: SolutionListUtilsTest

shouldFindBestSolutionRaiseAnExceptionIfTheComparatorIsNull
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldFindBestSolutionRaiseAnExceptionIfTheComparatorIsNull()
   :outertype: SolutionListUtilsTest

shouldFindBestSolutionRaiseAnExceptionIfTheSolutionListIsEmpty
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldFindBestSolutionRaiseAnExceptionIfTheSolutionListIsEmpty()
   :outertype: SolutionListUtilsTest

shouldFindBestSolutionRaiseAnExceptionIfTheSolutionListIsNull
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldFindBestSolutionRaiseAnExceptionIfTheSolutionListIsNull()
   :outertype: SolutionListUtilsTest

   ** Unit tests to method findBestSolution ***

shouldFindBestSolutionReturnTheLastOneIfThisIsTheBestSolutionInALastInAListWithFiveSolutions
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldFindBestSolutionReturnTheLastOneIfThisIsTheBestSolutionInALastInAListWithFiveSolutions()
   :outertype: SolutionListUtilsTest

shouldFindBestSolutionReturnTheSecondSolutionInTheListIfIsTheBestOufOfTwoSolutions
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldFindBestSolutionReturnTheSecondSolutionInTheListIfIsTheBestOufOfTwoSolutions()
   :outertype: SolutionListUtilsTest

shouldFindBestSolutionReturnTheSolutionInTheListWhenItContainsOneSolution
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldFindBestSolutionReturnTheSolutionInTheListWhenItContainsOneSolution()
   :outertype: SolutionListUtilsTest

shouldFindIndexOfBestSolutionRaiseAnExceptionIfTheComparatorIsNull
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldFindIndexOfBestSolutionRaiseAnExceptionIfTheComparatorIsNull()
   :outertype: SolutionListUtilsTest

shouldFindIndexOfBestSolutionRaiseAnExceptionIfTheSolutionListIsEmpty
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldFindIndexOfBestSolutionRaiseAnExceptionIfTheSolutionListIsEmpty()
   :outertype: SolutionListUtilsTest

shouldFindIndexOfBestSolutionRaiseAnExceptionIfTheSolutionListIsNull
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldFindIndexOfBestSolutionRaiseAnExceptionIfTheSolutionListIsNull()
   :outertype: SolutionListUtilsTest

   ** Unit tests to method findIndexOfBestSolution ***

shouldFindIndexOfBestSolutionReturn4IfTheBestSolutionIsTheLastInAListWithFiveSolutions
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldFindIndexOfBestSolutionReturn4IfTheBestSolutionIsTheLastInAListWithFiveSolutions()
   :outertype: SolutionListUtilsTest

shouldFindIndexOfBestSolutionReturnOneIfTheSecondSolutionItTheBestOutOfTwoSolutionInTheList
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldFindIndexOfBestSolutionReturnOneIfTheSecondSolutionItTheBestOutOfTwoSolutionInTheList()
   :outertype: SolutionListUtilsTest

shouldFindIndexOfBestSolutionReturnZeroIfTheFirstSolutionItTheBestOutOfTwoSolutionsInTheList
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldFindIndexOfBestSolutionReturnZeroIfTheFirstSolutionItTheBestOutOfTwoSolutionsInTheList()
   :outertype: SolutionListUtilsTest

shouldFindIndexOfBestSolutionReturnZeroIfTheListWhenItContainsOneSolution
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldFindIndexOfBestSolutionReturnZeroIfTheListWhenItContainsOneSolution()
   :outertype: SolutionListUtilsTest

shouldJMetalRandomGeneratorNotBeUsedWhenCustomRandomGeneratorProvidedInSelectNRandomDifferentSolutions
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldJMetalRandomGeneratorNotBeUsedWhenCustomRandomGeneratorProvidedInSelectNRandomDifferentSolutions()
   :outertype: SolutionListUtilsTest

shouldRestartRemoveTheRequestedPercentageOfSolutions
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldRestartRemoveTheRequestedPercentageOfSolutions()
   :outertype: SolutionListUtilsTest

   TODO

shouldSelectNRandomDifferentSolutionsRaiseAnExceptionIfTheListSizeIsOneAndTwoSolutionsAreRequested
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldSelectNRandomDifferentSolutionsRaiseAnExceptionIfTheListSizeIsOneAndTwoSolutionsAreRequested()
   :outertype: SolutionListUtilsTest

shouldSelectNRandomDifferentSolutionsRaiseAnExceptionIfTheSolutionListIsEmpty
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldSelectNRandomDifferentSolutionsRaiseAnExceptionIfTheSolutionListIsEmpty()
   :outertype: SolutionListUtilsTest

shouldSelectNRandomDifferentSolutionsRaiseAnExceptionIfTheSolutionListIsNull
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldSelectNRandomDifferentSolutionsRaiseAnExceptionIfTheSolutionListIsNull()
   :outertype: SolutionListUtilsTest

   ** Unit tests to method selectNRandomDifferentSolutions ***

shouldSelectNRandomDifferentSolutionsReturnASingleSolution
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldSelectNRandomDifferentSolutionsReturnASingleSolution()
   :outertype: SolutionListUtilsTest

shouldSelectNRandomDifferentSolutionsReturnTheCorrectListOfSolutions
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldSelectNRandomDifferentSolutionsReturnTheCorrectListOfSolutions()
   :outertype: SolutionListUtilsTest

   If the list contains 4 solutions, the result list must return all of them

shouldSelectNRandomDifferentSolutionsReturnTheCorrectNumberOfSolutions
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldSelectNRandomDifferentSolutionsReturnTheCorrectNumberOfSolutions()
   :outertype: SolutionListUtilsTest

shouldSelectNRandomDifferentSolutionsReturnTheSolutionSInTheListIfTheListContainsTwoSolutions
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldSelectNRandomDifferentSolutionsReturnTheSolutionSInTheListIfTheListContainsTwoSolutions()
   :outertype: SolutionListUtilsTest

shouldSolutionListsAreEqualsReturnIfTwoIdenticalSolutionListsAreCompared
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldSolutionListsAreEqualsReturnIfTwoIdenticalSolutionListsAreCompared()
   :outertype: SolutionListUtilsTest

shouldSolutionListsAreEqualsReturnIfTwoSolutionListsWithIdenticalSolutionsAreCompared
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldSolutionListsAreEqualsReturnIfTwoSolutionListsWithIdenticalSolutionsAreCompared()
   :outertype: SolutionListUtilsTest

shouldelectNRandomDifferentSolutionsRaiseAnExceptionIfTheListSizeIsTwoAndFourSolutionsAreRequested
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldelectNRandomDifferentSolutionsRaiseAnExceptionIfTheListSizeIsTwoAndFourSolutionsAreRequested()
   :outertype: SolutionListUtilsTest

