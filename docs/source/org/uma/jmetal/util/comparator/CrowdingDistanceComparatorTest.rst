.. java:import:: org.junit Before

.. java:import:: org.junit Test

.. java:import:: org.springframework.test.util ReflectionTestUtils

.. java:import:: org.uma.jmetal.solution BinarySolution

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util.solutionattribute.impl CrowdingDistance

CrowdingDistanceComparatorTest
==============================

.. java:package:: org.uma.jmetal.util.comparator
   :noindex:

.. java:type:: public class CrowdingDistanceComparatorTest

   :author: Antonio J. Nebro

Methods
-------
setup
^^^^^

.. java:method:: @Before public void setup()
   :outertype: CrowdingDistanceComparatorTest

shouldCompareReturnMinusOneIfSolutionBHasHigherDistance
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldCompareReturnMinusOneIfSolutionBHasHigherDistance()
   :outertype: CrowdingDistanceComparatorTest

shouldCompareReturnMinusOneIfTheSecondSolutionIsNull
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldCompareReturnMinusOneIfTheSecondSolutionIsNull()
   :outertype: CrowdingDistanceComparatorTest

shouldCompareReturnOneIfSolutionAHasLessDistance
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldCompareReturnOneIfSolutionAHasLessDistance()
   :outertype: CrowdingDistanceComparatorTest

shouldCompareReturnOneIfTheFirstSolutionIsNull
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldCompareReturnOneIfTheFirstSolutionIsNull()
   :outertype: CrowdingDistanceComparatorTest

shouldCompareReturnZeroIfBothSolutionsAreNull
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldCompareReturnZeroIfBothSolutionsAreNull()
   :outertype: CrowdingDistanceComparatorTest

shouldCompareReturnZeroIfBothSolutionsHaveNoCrowdingDistanceAttribute
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldCompareReturnZeroIfBothSolutionsHaveNoCrowdingDistanceAttribute()
   :outertype: CrowdingDistanceComparatorTest

shouldCompareReturnZeroIfBothSolutionsHaveTheSameDistance
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldCompareReturnZeroIfBothSolutionsHaveTheSameDistance()
   :outertype: CrowdingDistanceComparatorTest

