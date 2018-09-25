.. java:import:: org.junit After

.. java:import:: org.junit Before

.. java:import:: org.junit Test

.. java:import:: org.springframework.test.util ReflectionTestUtils

.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: java.util Comparator

RankingAndCrowdingDistanceComparatorTest
========================================

.. java:package:: org.uma.jmetal.util.comparator
   :noindex:

.. java:type:: public class RankingAndCrowdingDistanceComparatorTest

   :author: Antonio J. Nebro

Methods
-------
setup
^^^^^

.. java:method:: @Before public void setup()
   :outertype: RankingAndCrowdingDistanceComparatorTest

shouldCompareTwoNullSolutionsReturnZero
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldCompareTwoNullSolutionsReturnZero()
   :outertype: RankingAndCrowdingDistanceComparatorTest

shouldCompareWhenRankingYieldingAZeroReturnTheCrowdingDistanceValue
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldCompareWhenRankingYieldingAZeroReturnTheCrowdingDistanceValue()
   :outertype: RankingAndCrowdingDistanceComparatorTest

shouldCompareWithANullSolutionAsFirstArgumentReturnOne
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldCompareWithANullSolutionAsFirstArgumentReturnOne()
   :outertype: RankingAndCrowdingDistanceComparatorTest

shouldCompareWithANullSolutionAsSecondArgumentReturnMinusOne
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldCompareWithANullSolutionAsSecondArgumentReturnMinusOne()
   :outertype: RankingAndCrowdingDistanceComparatorTest

shouldCompareWithNullRankingAttributeSolutionAsFirstArgumentReturnOne
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldCompareWithNullRankingAttributeSolutionAsFirstArgumentReturnOne()
   :outertype: RankingAndCrowdingDistanceComparatorTest

shouldCompareWithRankingYieldingANonZeroValueReturnThatValue
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldCompareWithRankingYieldingANonZeroValueReturnThatValue()
   :outertype: RankingAndCrowdingDistanceComparatorTest

teardown
^^^^^^^^

.. java:method:: @After public void teardown()
   :outertype: RankingAndCrowdingDistanceComparatorTest

