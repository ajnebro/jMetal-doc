.. java:import:: org.junit Test

.. java:import:: org.uma.jmetal.problem DoubleProblem

.. java:import:: org.uma.jmetal.problem.impl AbstractDoubleProblem

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.solution.impl DefaultDoubleSolution

.. java:import:: java.util ArrayList

.. java:import:: java.util List

SolutionUtilsTest
=================

.. java:package:: org.uma.jmetal.util
   :noindex:

.. java:type:: public class SolutionUtilsTest

Methods
-------
shouldAverageDistanceToSolutionListWorkProperlyCaseA
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldAverageDistanceToSolutionListWorkProperlyCaseA()
   :outertype: SolutionUtilsTest

   Case A. Solution = [1], solutionList = [1]]

shouldAverageDistanceToSolutionListWorkProperlyCaseB
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldAverageDistanceToSolutionListWorkProperlyCaseB()
   :outertype: SolutionUtilsTest

   Case B. Solution = [1], solutionList = [[2]]

shouldAverageDistanceToSolutionListWorkProperlyCaseC
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldAverageDistanceToSolutionListWorkProperlyCaseC()
   :outertype: SolutionUtilsTest

   Case C. Solution = [1], solutionList = [[1], [2]]

shouldDistanceBetweenObjectivesWorkProperlyWithTwoSolutionsWithOneObjectiveCaseA
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldDistanceBetweenObjectivesWorkProperlyWithTwoSolutionsWithOneObjectiveCaseA()
   :outertype: SolutionUtilsTest

   Case A: the two solutions are the same

shouldDistanceBetweenObjectivesWorkProperlyWithTwoSolutionsWithOneObjectiveCaseB
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldDistanceBetweenObjectivesWorkProperlyWithTwoSolutionsWithOneObjectiveCaseB()
   :outertype: SolutionUtilsTest

   Case B: the two solutions are not the same

shouldDistanceBetweenObjectivesWorkProperlyWithTwoSolutionsWithTwoObjectivesCaseA
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldDistanceBetweenObjectivesWorkProperlyWithTwoSolutionsWithTwoObjectivesCaseA()
   :outertype: SolutionUtilsTest

   Case A: the two solutions are the same

shouldDistanceBetweenObjectivesWorkProperlyWithTwoSolutionsWithTwoObjectivesCaseB
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldDistanceBetweenObjectivesWorkProperlyWithTwoSolutionsWithTwoObjectivesCaseB()
   :outertype: SolutionUtilsTest

   Case B: the two solutions are not the same

