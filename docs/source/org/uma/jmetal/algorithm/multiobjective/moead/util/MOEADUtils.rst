.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: org.uma.jmetal.util.distance Distance

.. java:import:: org.uma.jmetal.util.distance.impl EuclideanDistanceBetweenSolutionAndASolutionListInObjectiveSpace

.. java:import:: org.uma.jmetal.util.pseudorandom JMetalRandom

.. java:import:: org.uma.jmetal.util.point.impl IdealPoint

.. java:import:: java.util ArrayList

.. java:import:: java.util List

MOEADUtils
==========

.. java:package:: org.uma.jmetal.algorithm.multiobjective.moead.util
   :noindex:

.. java:type:: public class MOEADUtils

   Utilities methods to used by MOEA/D

Methods
-------
distVector
^^^^^^^^^^

.. java:method:: public static double distVector(double[] vector1, double[] vector2)
   :outertype: MOEADUtils

getSubsetOfEvenlyDistributedSolutions
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public static <S extends Solution<?>> List<S> getSubsetOfEvenlyDistributedSolutions(List<S> solutionList, int newSolutionListSize)
   :outertype: MOEADUtils

   This methods select a subset of evenly spread solutions from a solution list. The implementation is based on the method described in the MOEA/D-DRA paper.

   :param solutionList:
   :param newSolutionListSize:
   :param <S>:

minFastSort
^^^^^^^^^^^

.. java:method:: public static void minFastSort(double[] x, int[] idx, int n, int m)
   :outertype: MOEADUtils

quickSort
^^^^^^^^^

.. java:method:: public static void quickSort(double[] array, int[] idx, int from, int to)
   :outertype: MOEADUtils

   Quick sort procedure (ascending order)

   :param array:
   :param idx:
   :param from:
   :param to:

randomPermutation
^^^^^^^^^^^^^^^^^

.. java:method:: public static void randomPermutation(int[] perm, int size)
   :outertype: MOEADUtils

