.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util.distance Distance

.. java:import:: org.uma.jmetal.util.distance.impl EuclideanDistanceBetweenSolutionsInObjectiveSpace

.. java:import:: org.uma.jmetal.util.neighborhood Neighborhood

.. java:import:: java.util ArrayList

.. java:import:: java.util List

KNearestNeighborhood
====================

.. java:package:: org.uma.jmetal.util.neighborhood.impl
   :noindex:

.. java:type:: public class KNearestNeighborhood<S extends Solution<?>> implements Neighborhood<S>

   This class implements a neighborhood that select the k-nearest solutions according to a distance measure. By default, the Euclidean distance between objectives is used.

   :param <S>:

Constructors
------------
KNearestNeighborhood
^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public KNearestNeighborhood(int neighborSize)
   :outertype: KNearestNeighborhood

KNearestNeighborhood
^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public KNearestNeighborhood(int neighborSize, Distance<S, S> distance)
   :outertype: KNearestNeighborhood

Methods
-------
getNeighbors
^^^^^^^^^^^^

.. java:method:: @Override public List<S> getNeighbors(List<S> solutionList, int solutionIndex)
   :outertype: KNearestNeighborhood

