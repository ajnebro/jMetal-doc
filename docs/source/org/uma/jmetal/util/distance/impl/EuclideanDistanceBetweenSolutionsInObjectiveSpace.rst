.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util.distance Distance

EuclideanDistanceBetweenSolutionsInObjectiveSpace
=================================================

.. java:package:: org.uma.jmetal.util.distance.impl
   :noindex:

.. java:type:: public class EuclideanDistanceBetweenSolutionsInObjectiveSpace<S extends Solution<?>> implements Distance<S, S>

   Class for calculating the Euclidean distance between two \ :java:ref:`Solution`\  objects in objective space.

   :author:

Methods
-------
getDistance
^^^^^^^^^^^

.. java:method:: @Override public double getDistance(S solution1, S solution2)
   :outertype: EuclideanDistanceBetweenSolutionsInObjectiveSpace

