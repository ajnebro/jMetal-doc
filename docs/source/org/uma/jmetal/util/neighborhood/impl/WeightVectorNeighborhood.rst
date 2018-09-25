.. java:import:: org.apache.commons.math3.ml.distance EuclideanDistance

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: org.uma.jmetal.util.neighborhood Neighborhood

.. java:import:: java.util ArrayList

.. java:import:: java.util List

.. java:import:: java.util StringTokenizer

WeightVectorNeighborhood
========================

.. java:package:: org.uma.jmetal.util.neighborhood.impl
   :noindex:

.. java:type:: public class WeightVectorNeighborhood<S> implements Neighborhood<S>

   This class implements a neighborhood based on the weight vectors of MOEA/D

   :author: Antonio J. Nebro

Constructors
------------
WeightVectorNeighborhood
^^^^^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public WeightVectorNeighborhood(int numberOfWeightVectors, int neighborSize)
   :outertype: WeightVectorNeighborhood

WeightVectorNeighborhood
^^^^^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public WeightVectorNeighborhood(int numberOfWeightVectors, int weightVectorSize, int neighborSize, String vectorFileName) throws FileNotFoundException
   :outertype: WeightVectorNeighborhood

Methods
-------
getNeighborSize
^^^^^^^^^^^^^^^

.. java:method:: public int getNeighborSize()
   :outertype: WeightVectorNeighborhood

getNeighborhood
^^^^^^^^^^^^^^^

.. java:method:: public int[][] getNeighborhood()
   :outertype: WeightVectorNeighborhood

getNeighbors
^^^^^^^^^^^^

.. java:method:: @Override public List<S> getNeighbors(List<S> solutionList, int solutionIndex)
   :outertype: WeightVectorNeighborhood

getNumberOfWeightVectors
^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public int getNumberOfWeightVectors()
   :outertype: WeightVectorNeighborhood

getWeightVector
^^^^^^^^^^^^^^^

.. java:method:: public double[][] getWeightVector()
   :outertype: WeightVectorNeighborhood

getWeightVectorSize
^^^^^^^^^^^^^^^^^^^

.. java:method:: public int getWeightVectorSize()
   :outertype: WeightVectorNeighborhood

