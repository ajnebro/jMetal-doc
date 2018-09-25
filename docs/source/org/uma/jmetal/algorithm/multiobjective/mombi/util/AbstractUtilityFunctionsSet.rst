.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: java.util ArrayList

.. java:import:: java.util List

.. java:import:: java.util StringTokenizer

AbstractUtilityFunctionsSet
===========================

.. java:package:: org.uma.jmetal.algorithm.multiobjective.mombi.util
   :noindex:

.. java:type:: @SuppressWarnings public abstract class AbstractUtilityFunctionsSet<S extends Solution<?>> implements Serializable

   :author: Juan J. Durillo Modified by Antonio J. Nebro
   :param <S>:

Constructors
------------
AbstractUtilityFunctionsSet
^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public AbstractUtilityFunctionsSet(double[][] weights)
   :outertype: AbstractUtilityFunctionsSet

AbstractUtilityFunctionsSet
^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public AbstractUtilityFunctionsSet(String file_path)
   :outertype: AbstractUtilityFunctionsSet

Methods
-------
evaluate
^^^^^^^^

.. java:method:: public List<Double> evaluate(S solution)
   :outertype: AbstractUtilityFunctionsSet

   Evaluates a solution using all the utility functions stored in this set

   :param solution:

evaluate
^^^^^^^^

.. java:method:: public abstract Double evaluate(S solution, int vector)
   :outertype: AbstractUtilityFunctionsSet

   Evaluates a solution using the i-th utility function stored in this set

   :param solution:
   :param vector:

getSize
^^^^^^^

.. java:method:: public int getSize()
   :outertype: AbstractUtilityFunctionsSet

   Returns the number of utility functions stored in this set

   :return: The number of vectors

getVectorSize
^^^^^^^^^^^^^

.. java:method:: public int getVectorSize()
   :outertype: AbstractUtilityFunctionsSet

   Returns the number of components for all weight vectors

getWeightVector
^^^^^^^^^^^^^^^

.. java:method:: public List<Double> getWeightVector(int index)
   :outertype: AbstractUtilityFunctionsSet

   Returns a given weight vector

loadWeightsFromFile
^^^^^^^^^^^^^^^^^^^

.. java:method:: public void loadWeightsFromFile(String filePath)
   :outertype: AbstractUtilityFunctionsSet

   Reads a set of weight vectors from a file. The expected format for the file is as follows. The first line should start with at least the following three tokens #   Any other token on this line will be ignored.  indicates how many weight vectors are included in this file  indicates how many component has each included vector Each of the following lines of the file represents a weight vector of at least  components If more components are provided, they will be ignored by the program

   :param filePath: The path in the file system of the file containing the weight vectors

