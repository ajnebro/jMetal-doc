.. java:import:: org.junit Test

.. java:import:: org.uma.jmetal.problem DoubleProblem

.. java:import:: org.uma.jmetal.problem.impl AbstractDoubleProblem

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.solution.impl DefaultDoubleSolution

.. java:import:: org.uma.jmetal.util.solutionattribute Ranking

.. java:import:: java.util ArrayList

.. java:import:: java.util Arrays

.. java:import:: java.util Collections

.. java:import:: java.util List

DominanceRankingTest
====================

.. java:package:: org.uma.jmetal.util.solutionattribute.impl
   :noindex:

.. java:type:: public class DominanceRankingTest

   :author: Antonio J. Nebro

Methods
-------
shouldRankingOfAPopulationWithFiveSolutionsWorkProperly
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldRankingOfAPopulationWithFiveSolutionsWorkProperly()
   :outertype: DominanceRankingTest

shouldRankingOfAPopulationWithThreeDominatedSolutionsReturnThreeSubfronts
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldRankingOfAPopulationWithThreeDominatedSolutionsReturnThreeSubfronts()
   :outertype: DominanceRankingTest

shouldRankingOfAPopulationWithTwoDominatedSolutionsReturnTwoSubfronts
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldRankingOfAPopulationWithTwoDominatedSolutionsReturnTwoSubfronts()
   :outertype: DominanceRankingTest

shouldRankingOfAPopulationWithTwoNonDominatedSolutionsReturnOneSubfront
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldRankingOfAPopulationWithTwoNonDominatedSolutionsReturnOneSubfront()
   :outertype: DominanceRankingTest

shouldTheRankingOfAnEmptyPopulationReturnOneSubfronts
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldTheRankingOfAnEmptyPopulationReturnOneSubfronts()
   :outertype: DominanceRankingTest

shouldTheRankingOfAnEmptyPopulationReturnZeroSubfronts
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldTheRankingOfAnEmptyPopulationReturnZeroSubfronts()
   :outertype: DominanceRankingTest

