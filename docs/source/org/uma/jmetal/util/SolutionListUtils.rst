.. java:import:: org.uma.jmetal.problem Problem

.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util.comparator DominanceComparator

.. java:import:: org.uma.jmetal.util.pseudorandom BoundedRandomGenerator

.. java:import:: org.uma.jmetal.util.pseudorandom JMetalRandom

.. java:import:: org.uma.jmetal.util.solutionattribute Ranking

.. java:import:: org.uma.jmetal.util.solutionattribute.impl DominanceRanking

SolutionListUtils
=================

.. java:package:: org.uma.jmetal.util
   :noindex:

.. java:type:: public class SolutionListUtils

   Created by Antonio J. Nebro on 04/10/14. Modified by Juanjo 13/03/15

Methods
-------
distanceMatrix
^^^^^^^^^^^^^^

.. java:method:: public static <S extends Solution<?>> double[][] distanceMatrix(List<S> solutionSet)
   :outertype: SolutionListUtils

   Returns a matrix with the euclidean distance between each pair of solutions in the population. Distances are measured in the objective space

   :param solutionSet:

fillPopulationWithNewSolutions
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public static <S> void fillPopulationWithNewSolutions(List<S> solutionList, Problem<S> problem, int maxListSize)
   :outertype: SolutionListUtils

   Fills a population with new solutions until its size is maxListSize

   :param solutionList: The list of solutions
   :param problem: The problem being solved
   :param maxListSize: The target size of the list
   :param <S>: The type of the solutions to be created

findBestSolution
^^^^^^^^^^^^^^^^

.. java:method:: public static <S> S findBestSolution(List<S> solutionList, Comparator<S> comparator)
   :outertype: SolutionListUtils

findIndexOfBestSolution
^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public static <S> int findIndexOfBestSolution(List<S> solutionList, Comparator<S> comparator)
   :outertype: SolutionListUtils

   Finds the index of the best solution in the list according to a comparator

   :param solutionList:
   :param comparator:
   :return: The index of the best solution

findIndexOfWorstSolution
^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public static <S> int findIndexOfWorstSolution(List<? extends S> solutionList, Comparator<S> comparator)
   :outertype: SolutionListUtils

   Finds the index of the worst solution in the list according to a comparator

   :param solutionList:
   :param comparator:
   :return: The index of the best solution

findWorstSolution
^^^^^^^^^^^^^^^^^

.. java:method:: public <S> S findWorstSolution(Collection<S> solutionList, Comparator<S> comparator)
   :outertype: SolutionListUtils

getInvertedFront
^^^^^^^^^^^^^^^^

.. java:method:: @SuppressWarnings public static <S extends Solution<?>> List<S> getInvertedFront(List<S> solutionSet)
   :outertype: SolutionListUtils

   This method receives a normalized list of non-dominated solutions and return the inverted one. This operation is needed for minimization problem

   :param solutionSet: The front to invert
   :return: The inverted front

getNondominatedSolutions
^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public static <S extends Solution<?>> List<S> getNondominatedSolutions(List<S> solutionList)
   :outertype: SolutionListUtils

getNormalizedFront
^^^^^^^^^^^^^^^^^^

.. java:method:: public static List<Solution<?>> getNormalizedFront(List<Solution<?>> solutionList, List<Double> maximumValue, List<Double> minimumValue)
   :outertype: SolutionListUtils

   This method receives a list of non-dominated solutions and maximum and minimum values of the objectives, and returns a the normalized set of solutions.

   :param solutionList: A list of non-dominated solutions
   :param maximumValue: The maximum values of the objectives
   :param minimumValue: The minimum values of the objectives
   :return: the normalized list of non-dominated solutions

getObjectiveArrayFromSolutionList
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public static <S extends Solution<?>> double[] getObjectiveArrayFromSolutionList(List<S> solutionList, int objective)
   :outertype: SolutionListUtils

   Given a solution list and the identifier of an objective (0, 1, etc), returns an array with the values of that objective in all the solutions of the list

   :param solutionList:
   :param objective:
   :param <S>:

isSolutionDominatedBySolutionList
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public static <S extends Solution<?>> boolean isSolutionDominatedBySolutionList(S solution, List<? extends S> solutionSet)
   :outertype: SolutionListUtils

removeSolutionsFromList
^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public static <S> void removeSolutionsFromList(List<S> solutionList, int numberOfSolutionsToRemove)
   :outertype: SolutionListUtils

   Removes a number of solutions from a list

   :param solutionList: The list of solutions
   :param numberOfSolutionsToRemove:

restart
^^^^^^^

.. java:method:: public static <S> void restart(List<S> solutionList, Problem<S> problem, int percentageOfSolutionsToRemove)
   :outertype: SolutionListUtils

   This methods takes a list of solutions, removes a percentage of its solutions, and it is filled with new random generated solutions

   :param solutionList:
   :param problem:
   :param percentageOfSolutionsToRemove:

selectNRandomDifferentSolutions
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public static <S> List<S> selectNRandomDifferentSolutions(int numberOfSolutionsToBeReturned, List<S> solutionList)
   :outertype: SolutionListUtils

   This method receives a normalized list of non-dominated solutions and return the inverted one. This operation is needed for minimization problem

   :param solutionList: The front to invert
   :return: The inverted front

selectNRandomDifferentSolutions
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public static <S> List<S> selectNRandomDifferentSolutions(int numberOfSolutionsToBeReturned, List<S> solutionList, BoundedRandomGenerator<Integer> randomGenerator)
   :outertype: SolutionListUtils

   This method receives a normalized list of non-dominated solutions and return the inverted one. This operation is needed for minimization problem

   :param solutionList: The front to invert
   :param randomGenerator: The random generator to use
   :return: The inverted front

solutionListsAreEquals
^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public static <S> boolean solutionListsAreEquals(List<S> solutionList, List<S> newSolutionList)
   :outertype: SolutionListUtils

   Compares two solution lists to determine if both are equals

   :param solutionList: A \ ``Solution list``\
   :param newSolutionList: A \ ``Solution list``\
   :return: true if both are contains the same solutions, false in other case

writeObjectivesToMatrix
^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public static <S extends Solution<?>> double[][] writeObjectivesToMatrix(List<S> solutionList)
   :outertype: SolutionListUtils

