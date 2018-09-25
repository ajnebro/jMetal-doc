.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util.distance Distance

CosineDistanceBetweenSolutionsInObjectiveSpace
==============================================

.. java:package:: org.uma.jmetal.util.distance.impl
   :noindex:

.. java:type:: public class CosineDistanceBetweenSolutionsInObjectiveSpace<S extends Solution<?>> implements Distance<S, S>

   Class for calculating the cosine distance between two \ :java:ref:`Solution`\  objects in objective space.

   :author:

Constructors
------------
CosineDistanceBetweenSolutionsInObjectiveSpace
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public CosineDistanceBetweenSolutionsInObjectiveSpace(S referencePoint)
   :outertype: CosineDistanceBetweenSolutionsInObjectiveSpace

Methods
-------
getDistance
^^^^^^^^^^^

.. java:method:: @Override public double getDistance(S solution1, S solution2)
   :outertype: CosineDistanceBetweenSolutionsInObjectiveSpace

