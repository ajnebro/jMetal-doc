.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util.distance Distance

.. java:import:: java.util List

EuclideanDistanceBetweenSolutionAndASolutionListInObjectiveSpace
================================================================

.. java:package:: org.uma.jmetal.util.distance.impl
   :noindex:

.. java:type:: public class EuclideanDistanceBetweenSolutionAndASolutionListInObjectiveSpace<S extends Solution<Double>, L extends List<S>> implements Distance<S, L>

   Class for calculating the Euclidean distance between a \ :java:ref:`Solution`\  object a list of \ :java:ref:`Solution`\  objects in objective space.

   :author:

Constructors
------------
EuclideanDistanceBetweenSolutionAndASolutionListInObjectiveSpace
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public EuclideanDistanceBetweenSolutionAndASolutionListInObjectiveSpace()
   :outertype: EuclideanDistanceBetweenSolutionAndASolutionListInObjectiveSpace

Methods
-------
getDistance
^^^^^^^^^^^

.. java:method:: @Override public double getDistance(S solution, L solutionList)
   :outertype: EuclideanDistanceBetweenSolutionAndASolutionListInObjectiveSpace

