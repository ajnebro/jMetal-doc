.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util.distance Distance

EuclideanDistanceBetweenSolutionsInSolutionSpace
================================================

.. java:package:: org.uma.jmetal.util.distance.impl
   :noindex:

.. java:type:: public class EuclideanDistanceBetweenSolutionsInSolutionSpace<S extends Solution<Double>> implements Distance<S, S>

   Class for calculating the Euclidean distance between two \ :java:ref:`DoubleSolution`\  objects in solution space.

   :author:

Methods
-------
getDistance
^^^^^^^^^^^

.. java:method:: @Override public double getDistance(S solution1, S solution2)
   :outertype: EuclideanDistanceBetweenSolutionsInSolutionSpace

