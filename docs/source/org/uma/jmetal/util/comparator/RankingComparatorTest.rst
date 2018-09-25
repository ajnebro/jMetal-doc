.. java:import:: org.junit Before

.. java:import:: org.junit Test

.. java:import:: org.springframework.test.util ReflectionTestUtils

.. java:import:: org.uma.jmetal.solution BinarySolution

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util.solutionattribute Ranking

RankingComparatorTest
=====================

.. java:package:: org.uma.jmetal.util.comparator
   :noindex:

.. java:type:: public class RankingComparatorTest

   :author: Antonio J. Nebro

Methods
-------
setup
^^^^^

.. java:method:: @Before public void setup()
   :outertype: RankingComparatorTest

shouldCompareReturnMinusOneIfSolutionAHasLessRanking
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldCompareReturnMinusOneIfSolutionAHasLessRanking()
   :outertype: RankingComparatorTest

shouldCompareReturnMinusOneIfTheSecondSolutionIsNull
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldCompareReturnMinusOneIfTheSecondSolutionIsNull()
   :outertype: RankingComparatorTest

shouldCompareReturnOneIfSolutionBHasLessRanking
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldCompareReturnOneIfSolutionBHasLessRanking()
   :outertype: RankingComparatorTest

shouldCompareReturnOneIfTheFirstSolutionIsNull
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldCompareReturnOneIfTheFirstSolutionIsNull()
   :outertype: RankingComparatorTest

shouldCompareReturnZeroIfBothSolutionsAreNull
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldCompareReturnZeroIfBothSolutionsAreNull()
   :outertype: RankingComparatorTest

shouldCompareReturnZeroIfBothSolutionsHaveNoRankingAttribute
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldCompareReturnZeroIfBothSolutionsHaveNoRankingAttribute()
   :outertype: RankingComparatorTest

shouldCompareReturnZeroIfBothSolutionsHaveTheSameRanking
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldCompareReturnZeroIfBothSolutionsHaveTheSameRanking()
   :outertype: RankingComparatorTest

