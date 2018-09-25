.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: java.io BufferedReader

.. java:import:: java.io FileInputStream

.. java:import:: java.io InputStream

.. java:import:: java.io InputStreamReader

.. java:import:: java.util StringTokenizer

.. java:import:: java.util Vector

WeightVectors
=============

.. java:package:: org.uma.jmetal.algorithm.multiobjective.wasfga.util
   :noindex:

.. java:type:: public class WeightVectors

   :author: Rubén Saborido Infantes This class offers different methods to manipulate weight vectors.

Methods
-------
initializeUniformlyInTwoDimensions
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public static double[][] initializeUniformlyInTwoDimensions(double epsilon, int numberOfWeights)
   :outertype: WeightVectors

   Generate uniform weight vectors in two dimension

   :param epsilon: Distance between each component of the weight vector
   :param numberOfWeights: Number of weight vectors to generate
   :return: A set of weight vectors

invert
^^^^^^

.. java:method:: public static double[][] invert(double[][] weights, boolean normalize)
   :outertype: WeightVectors

   Calculate the inverse of a set of weight vectors

   :param weights: A set of weight vectors
   :param normalize: True if the weights should be normalize by the sum of the components
   :return: A set of weight vectors

readFromFile
^^^^^^^^^^^^

.. java:method:: public static double[][] readFromFile(String filePath)
   :outertype: WeightVectors

   Read a set of weight vector from a file

   :param filePath: A file containing the weight vectors
   :return: A set of weight vectors

readFromResourcesInJMetal
^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public static double[][] readFromResourcesInJMetal(String filePath)
   :outertype: WeightVectors

   Read a set of weight vector from a file in the resources folder in jMetal

   :param filePath: The name of file in the resources folder of jMetal
   :return: A set of weight vectors

validate
^^^^^^^^

.. java:method:: public static boolean validate(double[][] weights, int numberOfComponents)
   :outertype: WeightVectors

   Validate if the number of components of all weight vectors has the expected dimensionality.

   :param weights: Weight vectors to validate
   :param numberOfComponents: Number of components each weight vector must have
   :return: True if the weight vectors are correct, False if the weight vectors are incorrect

