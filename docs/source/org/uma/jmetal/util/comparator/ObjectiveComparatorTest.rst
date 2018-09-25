.. java:import:: org.junit Rule

.. java:import:: org.junit Test

.. java:import:: org.junit.rules ExpectedException

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util JMetalException

ObjectiveComparatorTest
=======================

.. java:package:: org.uma.jmetal.util.comparator
   :noindex:

.. java:type:: public class ObjectiveComparatorTest

   :author: Antonio J. Nebro

Fields
------
exception
^^^^^^^^^

.. java:field:: @Rule public ExpectedException exception
   :outertype: ObjectiveComparatorTest

Methods
-------
shouldCompareRaiseAnExceptionIfSolution1HasLessObjectivesThanTheOneRequested
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldCompareRaiseAnExceptionIfSolution1HasLessObjectivesThanTheOneRequested()
   :outertype: ObjectiveComparatorTest

shouldCompareRaiseAnExceptionIfSolution2HasLessObjectivesThanTheOneRequested
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldCompareRaiseAnExceptionIfSolution2HasLessObjectivesThanTheOneRequested()
   :outertype: ObjectiveComparatorTest

shouldCompareReturnMinusOneIfTheObjectiveOfSolution1IsGreaterInDescendingOrder
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldCompareReturnMinusOneIfTheObjectiveOfSolution1IsGreaterInDescendingOrder()
   :outertype: ObjectiveComparatorTest

shouldCompareReturnMinusOneIfTheObjectiveOfSolution1IsLower
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldCompareReturnMinusOneIfTheObjectiveOfSolution1IsLower()
   :outertype: ObjectiveComparatorTest

shouldCompareReturnMinusOneIfTheSecondSolutionIsNull
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldCompareReturnMinusOneIfTheSecondSolutionIsNull()
   :outertype: ObjectiveComparatorTest

shouldCompareReturnOneIfTheFirstSolutionIsNull
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldCompareReturnOneIfTheFirstSolutionIsNull()
   :outertype: ObjectiveComparatorTest

shouldCompareReturnOneIfTheObjectiveOfSolution2IsGreaterInDescendingOrder
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldCompareReturnOneIfTheObjectiveOfSolution2IsGreaterInDescendingOrder()
   :outertype: ObjectiveComparatorTest

shouldCompareReturnOneIfTheObjectiveOfSolution2IsLower
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldCompareReturnOneIfTheObjectiveOfSolution2IsLower()
   :outertype: ObjectiveComparatorTest

shouldCompareReturnZeroIfBothSolutionsAreNull
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldCompareReturnZeroIfBothSolutionsAreNull()
   :outertype: ObjectiveComparatorTest

shouldCompareReturnZeroIfTheObjectiveOfTheSolutionsIsTheSame
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldCompareReturnZeroIfTheObjectiveOfTheSolutionsIsTheSame()
   :outertype: ObjectiveComparatorTest

