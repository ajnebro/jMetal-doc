.. java:import:: org.hamcrest Matchers

.. java:import:: org.junit Rule

.. java:import:: org.junit Test

.. java:import:: org.junit.rules ExpectedException

.. java:import:: org.springframework.test.util ReflectionTestUtils

.. java:import:: org.uma.jmetal.solution BinarySolution

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.solution IntegerSolution

.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: java.util ArrayList

.. java:import:: java.util List

NaryRandomSelectionTest
=======================

.. java:package:: org.uma.jmetal.operator.impl.selection
   :noindex:

.. java:type:: public class NaryRandomSelectionTest

   :author: Antonio J. Nebro

Fields
------
exception
^^^^^^^^^

.. java:field:: @Rule public ExpectedException exception
   :outertype: NaryRandomSelectionTest

Methods
-------
shouldDefaultConstructorReturnASingleSolution
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldDefaultConstructorReturnASingleSolution()
   :outertype: NaryRandomSelectionTest

shouldExecuteRaiseAnExceptionIfTheListSizeIsOneAndTwoSolutionsAreRequested
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldExecuteRaiseAnExceptionIfTheListSizeIsOneAndTwoSolutionsAreRequested()
   :outertype: NaryRandomSelectionTest

shouldExecuteRaiseAnExceptionIfTheListSizeIsTwoAndFourSolutionsAreRequested
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldExecuteRaiseAnExceptionIfTheListSizeIsTwoAndFourSolutionsAreRequested()
   :outertype: NaryRandomSelectionTest

shouldExecuteRaiseAnExceptionIfTheSolutionListIsEmpty
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldExecuteRaiseAnExceptionIfTheSolutionListIsEmpty()
   :outertype: NaryRandomSelectionTest

shouldExecuteRaiseAnExceptionIfTheSolutionListIsNull
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldExecuteRaiseAnExceptionIfTheSolutionListIsNull()
   :outertype: NaryRandomSelectionTest

shouldExecuteReturnTheCorrectNumberOfSolutions
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldExecuteReturnTheCorrectNumberOfSolutions()
   :outertype: NaryRandomSelectionTest

shouldExecuteReturnTheSolutionInTheListIfTheListContainsASolution
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldExecuteReturnTheSolutionInTheListIfTheListContainsASolution()
   :outertype: NaryRandomSelectionTest

shouldExecuteReturnTheSolutionSInTheListIfTheListContainsTwoSolutions
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldExecuteReturnTheSolutionSInTheListIfTheListContainsTwoSolutions()
   :outertype: NaryRandomSelectionTest

shouldNonDefaultConstructorReturnTheCorrectNumberOfSolutions
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldNonDefaultConstructorReturnTheCorrectNumberOfSolutions()
   :outertype: NaryRandomSelectionTest

shouldSelectNRandomDifferentSolutionsReturnTheCorrectListOfSolutions
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldSelectNRandomDifferentSolutionsReturnTheCorrectListOfSolutions()
   :outertype: NaryRandomSelectionTest

   If the list contains 4 solutions, the result list must return all of them

