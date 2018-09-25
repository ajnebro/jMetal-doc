.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util.pseudorandom JMetalRandom

.. java:import:: org.uma.jmetal.util.pseudorandom RandomGenerator

.. java:import:: java.util Comparator

.. java:import:: java.util List

.. java:import:: java.util.function BinaryOperator

SolutionUtils
=============

.. java:package:: org.uma.jmetal.util
   :noindex:

.. java:type:: public class SolutionUtils

   Created by Antonio J. Nebro on 6/12/14.

Methods
-------
averageDistanceToSolutionList
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public static <S extends Solution<?>> double averageDistanceToSolutionList(S solution, List<S> solutionList)
   :outertype: SolutionUtils

   Returns the average euclidean distance of a solution to the solutions of a list.

distanceBetweenObjectives
^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public static <S extends Solution<?>> double distanceBetweenObjectives(S firstSolution, S secondSolution)
   :outertype: SolutionUtils

   Returns the euclidean distance between a pair of solutions in the objective space

distanceBetweenSolutionsInObjectiveSpace
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public static double distanceBetweenSolutionsInObjectiveSpace(DoubleSolution solutionI, DoubleSolution solutionJ)
   :outertype: SolutionUtils

   Returns the distance between two solutions in the search space.

   :param solutionI: The first \ ``Solution``\ .
   :param solutionJ: The second \ ``Solution``\ .
   :return: the distance between solutions.

distanceToSolutionListInSolutionSpace
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public static double distanceToSolutionListInSolutionSpace(DoubleSolution solution, List<DoubleSolution> solutionList)
   :outertype: SolutionUtils

   Returns the minimum distance from a \ ``Solution``\  to a SolutionSet according to
   the encodings.variable values.

   :param solution: The \ ``Solution``\ .
   :param solutionList: The \ ``List>``\ .
   :return: The minimum distance between solution and the set.

getBestSolution
^^^^^^^^^^^^^^^

.. java:method:: public static <S extends Solution<?>> S getBestSolution(S solution1, S solution2, Comparator<S> comparator)
   :outertype: SolutionUtils

   Return the best solution between those passed as arguments. If they are equal or incomparable one of them is chosen randomly.

   :return: The best solution

getBestSolution
^^^^^^^^^^^^^^^

.. java:method:: public static <S extends Solution<?>> S getBestSolution(S solution1, S solution2, Comparator<S> comparator, RandomGenerator<Double> randomGenerator)
   :outertype: SolutionUtils

   Return the best solution between those passed as arguments. If they are equal or incomparable one of them is chosen randomly.

   :param randomGenerator: \ :java:ref:`RandomGenerator`\  for the equality case
   :return: The best solution

getBestSolution
^^^^^^^^^^^^^^^

.. java:method:: public static <S extends Solution<?>> S getBestSolution(S solution1, S solution2, Comparator<S> comparator, BinaryOperator<S> equalityPolicy)
   :outertype: SolutionUtils

   Return the best solution between those passed as arguments. If they are equal or incomparable one of them is chosen based on the given policy.

   :return: The best solution

