.. java:import:: org.junit Rule

.. java:import:: org.junit Test

.. java:import:: org.junit.rules ExpectedException

.. java:import:: org.springframework.test.util ReflectionTestUtils

.. java:import:: org.uma.jmetal.problem DoubleProblem

.. java:import:: org.uma.jmetal.problem IntegerProblem

.. java:import:: org.uma.jmetal.problem.impl AbstractDoubleProblem

.. java:import:: org.uma.jmetal.problem.impl AbstractIntegerProblem

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.solution IntegerSolution

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: org.uma.jmetal.util.front Front

.. java:import:: org.uma.jmetal.util.point Point

.. java:import:: org.uma.jmetal.util.point.impl ArrayPoint

.. java:import:: org.uma.jmetal.util.point.util.comparator LexicographicalPointComparator

.. java:import:: java.io FileNotFoundException

.. java:import:: java.util ArrayList

.. java:import:: java.util Arrays

.. java:import:: java.util List

ArrayFrontTest
==============

.. java:package:: org.uma.jmetal.util.front.imp
   :noindex:

.. java:type:: public class ArrayFrontTest

   :author: Antonio J. Nebro

Fields
------
exception
^^^^^^^^^

.. java:field:: @Rule public ExpectedException exception
   :outertype: ArrayFrontTest

Methods
-------
shouldConstructorCreateAnArranFrontFromAFileContainingA2DFront
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldConstructorCreateAnArranFrontFromAFileContainingA2DFront() throws FileNotFoundException
   :outertype: ArrayFrontTest

shouldConstructorCreateAnArranFrontFromAFileContainingA3DFront
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldConstructorCreateAnArranFrontFromAFileContainingA3DFront() throws FileNotFoundException
   :outertype: ArrayFrontTest

shouldCreateAnArrayFrontFromAListOfSolutionsHavingOneDoubleSolutionObject
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldCreateAnArrayFrontFromAListOfSolutionsHavingOneDoubleSolutionObject()
   :outertype: ArrayFrontTest

shouldCreateAnArrayFrontFromAListOfSolutionsHavingOneSingleSolutionObject
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldCreateAnArrayFrontFromAListOfSolutionsHavingOneSingleSolutionObject()
   :outertype: ArrayFrontTest

shouldCreateAnArrayFrontFromAListOfSolutionsHavingTwoDoubleSolutionObject
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldCreateAnArrayFrontFromAListOfSolutionsHavingTwoDoubleSolutionObject()
   :outertype: ArrayFrontTest

shouldCreateAnArrayFrontFromANullFrontRaiseAnException
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldCreateAnArrayFrontFromANullFrontRaiseAnException()
   :outertype: ArrayFrontTest

shouldCreateAnArrayFrontFromANullListRaiseAnAnException
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldCreateAnArrayFrontFromANullListRaiseAnAnException()
   :outertype: ArrayFrontTest

shouldCreateAnArrayFrontFromASolutionListResultInTwoEqualsFronts
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldCreateAnArrayFrontFromASolutionListResultInTwoEqualsFronts()
   :outertype: ArrayFrontTest

shouldCreateAnArrayFrontFromAnEmptyFrontRaiseAnException
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldCreateAnArrayFrontFromAnEmptyFrontRaiseAnException()
   :outertype: ArrayFrontTest

shouldCreateAnArrayFrontFromAnEmptyListRaiseAnException
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldCreateAnArrayFrontFromAnEmptyListRaiseAnException()
   :outertype: ArrayFrontTest

shouldCreateAnArrayFrontFromAnotherFrontResultInTwoEqualsFrontssss
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldCreateAnArrayFrontFromAnotherFrontResultInTwoEqualsFrontssss()
   :outertype: ArrayFrontTest

shouldCreateInputStreamThrownAnExceptionIfFileDoesNotExist
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldCreateInputStreamThrownAnExceptionIfFileDoesNotExist() throws FileNotFoundException
   :outertype: ArrayFrontTest

shouldDefaultConstructorCreateAnEmptyArrayFront
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldDefaultConstructorCreateAnEmptyArrayFront()
   :outertype: ArrayFrontTest

shouldEqualsReturnFalseIfPointDimensionsOfTheFrontsIsDifferent
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldEqualsReturnFalseIfPointDimensionsOfTheFrontsIsDifferent()
   :outertype: ArrayFrontTest

shouldEqualsReturnFalseIfTheArgumentIsFromAWrongClass
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @SuppressWarnings @Test public void shouldEqualsReturnFalseIfTheArgumentIsFromAWrongClass()
   :outertype: ArrayFrontTest

shouldEqualsReturnFalseIfTheArgumentIsNull
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldEqualsReturnFalseIfTheArgumentIsNull()
   :outertype: ArrayFrontTest

shouldEqualsReturnFalseIfTheComparedFrontHasADifferentNumberOfPoints
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldEqualsReturnFalseIfTheComparedFrontHasADifferentNumberOfPoints()
   :outertype: ArrayFrontTest

shouldEqualsReturnFalseIfTheFrontsAreDifferent
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldEqualsReturnFalseIfTheFrontsAreDifferent()
   :outertype: ArrayFrontTest

shouldEqualsReturnTrueIfTheArgumentIsEqual
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldEqualsReturnTrueIfTheArgumentIsEqual()
   :outertype: ArrayFrontTest

shouldEqualsReturnTrueIfTheArgumentIsTheSameObject
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldEqualsReturnTrueIfTheArgumentIsTheSameObject()
   :outertype: ArrayFrontTest

shouldGetPointRaiseAnExceptionWhenTheIndexIsGreaterThanTheFrontSize
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldGetPointRaiseAnExceptionWhenTheIndexIsGreaterThanTheFrontSize()
   :outertype: ArrayFrontTest

shouldGetPointRaiseAnExceptionWhenTheIndexIsNegative
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldGetPointRaiseAnExceptionWhenTheIndexIsNegative()
   :outertype: ArrayFrontTest

shouldGetPointReturnTheCorrectObject
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldGetPointReturnTheCorrectObject()
   :outertype: ArrayFrontTest

shouldReadFrontAFileWithOnePointCreateTheCorrectFront
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldReadFrontAFileWithOnePointCreateTheCorrectFront() throws FileNotFoundException
   :outertype: ArrayFrontTest

   Test using a file containing: 1.0 2.0 -3.0

shouldReadFrontAnEmptyFileCreateAnEmptyFront
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldReadFrontAnEmptyFileCreateAnEmptyFront() throws FileNotFoundException
   :outertype: ArrayFrontTest

shouldReadFrontFourPointsCreateTheCorrectFront
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldReadFrontFourPointsCreateTheCorrectFront() throws FileNotFoundException, JMetalException
   :outertype: ArrayFrontTest

   Test using a file containing: 1 2 3 4 5 6 7 8 9 10 11 12 -1 -2 -3 -4

shouldReadFrontWithALineContainingWrongDataRaiseAnException
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldReadFrontWithALineContainingWrongDataRaiseAnException() throws FileNotFoundException, JMetalException
   :outertype: ArrayFrontTest

   Test using a file containing: 3.0 2.3 asdfg

shouldReadFrontWithALineWithALineMissingDataRaiseAnException
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldReadFrontWithALineWithALineMissingDataRaiseAnException() throws FileNotFoundException, JMetalException
   :outertype: ArrayFrontTest

   Test using a file containing: -30 234.234 90.25 15 -5.23

shouldSetPointAssignTheCorrectObject
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldSetPointAssignTheCorrectObject()
   :outertype: ArrayFrontTest

shouldSetPointRaiseAnExceptionWhenTheIndexIsGreaterThanTheFrontSize
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldSetPointRaiseAnExceptionWhenTheIndexIsGreaterThanTheFrontSize()
   :outertype: ArrayFrontTest

shouldSetPointRaiseAnExceptionWhenTheIndexIsNegative
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldSetPointRaiseAnExceptionWhenTheIndexIsNegative()
   :outertype: ArrayFrontTest

shouldSetPointRaiseAnExceptionWhenThePointIsNull
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldSetPointRaiseAnExceptionWhenThePointIsNull()
   :outertype: ArrayFrontTest

shouldSortReturnAnOrderedFront
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldSortReturnAnOrderedFront()
   :outertype: ArrayFrontTest

