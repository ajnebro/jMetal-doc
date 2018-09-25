.. java:import:: org.junit Rule

.. java:import:: org.junit Test

.. java:import:: org.junit.rules ExpectedException

.. java:import:: org.uma.jmetal.solution BinarySolution

.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util JMetalException

DominanceComparatorTest
=======================

.. java:package:: org.uma.jmetal.util.comparator
   :noindex:

.. java:type:: public class DominanceComparatorTest

   :author: Antonio J. Nebro

Fields
------
exception
^^^^^^^^^

.. java:field:: @Rule public ExpectedException exception
   :outertype: DominanceComparatorTest

Methods
-------
shouldCompareRaiseAnExceptionIfTheFirstSolutionIsNull
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldCompareRaiseAnExceptionIfTheFirstSolutionIsNull()
   :outertype: DominanceComparatorTest

shouldCompareRaiseAnExceptionIfTheSecondSolutionIsNull
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldCompareRaiseAnExceptionIfTheSecondSolutionIsNull()
   :outertype: DominanceComparatorTest

shouldCompareRaiseAnExceptionIfTheSolutionsHaveNotTheSameNumberOfObjectives
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldCompareRaiseAnExceptionIfTheSolutionsHaveNotTheSameNumberOfObjectives()
   :outertype: DominanceComparatorTest

shouldCompareReturnMinusOneIfTheFirstSolutionDominatesTheSecondOneCaseA
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldCompareReturnMinusOneIfTheFirstSolutionDominatesTheSecondOneCaseA()
   :outertype: DominanceComparatorTest

   Case A: solution1 has objectives [-1.0, 5.0, 9.0] and solution2 has [2.0, 6.0, 15.0]

shouldCompareReturnMinusOneIfTheFirstSolutionDominatesTheSecondOneCaseB
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldCompareReturnMinusOneIfTheFirstSolutionDominatesTheSecondOneCaseB()
   :outertype: DominanceComparatorTest

   Case B: solution1 has objectives [-1.0, 5.0, 9.0] and solution2 has [-1.0, 5.0, 10.0]

shouldCompareReturnMinusOneIfTheTwoSolutionsHasOneObjectiveAndTheFirstOneIsLower
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldCompareReturnMinusOneIfTheTwoSolutionsHasOneObjectiveAndTheFirstOneIsLower()
   :outertype: DominanceComparatorTest

shouldCompareReturnOneIfTheSecondSolutionDominatesTheFirstOneCaseC
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldCompareReturnOneIfTheSecondSolutionDominatesTheFirstOneCaseC()
   :outertype: DominanceComparatorTest

   Case C: solution1 has objectives [-1.0, 5.0, 9.0] and solution2 has [-2.0, 5.0, 9.0]

shouldCompareReturnOneIfTheSecondSolutionDominatesTheFirstOneCaseD
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldCompareReturnOneIfTheSecondSolutionDominatesTheFirstOneCaseD()
   :outertype: DominanceComparatorTest

   Case D: solution1 has objectives [-1.0, 5.0, 9.0] and solution2 has [-1.0, 5.0, 8.0]

shouldCompareReturnOneIfTheTwoSolutionsHasOneObjectiveAndTheSecondOneIsLower
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldCompareReturnOneIfTheTwoSolutionsHasOneObjectiveAndTheSecondOneIsLower()
   :outertype: DominanceComparatorTest

shouldCompareReturnTheValueReturnedByTheConstraintViolationComparator
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldCompareReturnTheValueReturnedByTheConstraintViolationComparator()
   :outertype: DominanceComparatorTest

shouldCompareReturnZeroIfTheTwoSolutionsHaveOneObjectiveWithTheSameValue
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldCompareReturnZeroIfTheTwoSolutionsHaveOneObjectiveWithTheSameValue()
   :outertype: DominanceComparatorTest

