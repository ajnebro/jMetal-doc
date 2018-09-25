.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: org.uma.jmetal.util.neighborhood Neighborhood

.. java:import:: org.uma.jmetal.util.pseudorandom BoundedRandomGenerator

.. java:import:: org.uma.jmetal.util.pseudorandom JMetalRandom

.. java:import:: java.util ArrayList

.. java:import:: java.util List

AdaptiveRandomNeighborhood
==========================

.. java:package:: org.uma.jmetal.util.neighborhood.impl
   :noindex:

.. java:type:: @SuppressWarnings public class AdaptiveRandomNeighborhood<S> implements Neighborhood<S>

   This class implements the adaptive random neighborhood (topology) defined by M. Clerc. Each solution in a solution list must have a neighborhood composed by it itself and K random selected neighbors (the same solution can be chosen several times).

   :author: Antonio J. Nebro

Constructors
------------
AdaptiveRandomNeighborhood
^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public AdaptiveRandomNeighborhood(int solutionListSize, int numberOfRandomNeighbours)
   :outertype: AdaptiveRandomNeighborhood

   Constructor

   :param solutionListSize: The expected size of the list of solutions
   :param numberOfRandomNeighbours: The number of neighbors per solution

AdaptiveRandomNeighborhood
^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public AdaptiveRandomNeighborhood(int solutionListSize, int numberOfRandomNeighbours, BoundedRandomGenerator<Integer> randomGenerator)
   :outertype: AdaptiveRandomNeighborhood

   Constructor

   :param solutionListSize: The expected size of the list of solutions
   :param numberOfRandomNeighbours: The number of neighbors per solution
   :param randomGenerator: the \ :java:ref:`BoundedRandomGenerator`\  to use for the randomisation

Methods
-------
getNeighbors
^^^^^^^^^^^^

.. java:method:: @Override public List<S> getNeighbors(List<S> solutionList, int solutionIndex)
   :outertype: AdaptiveRandomNeighborhood

recompute
^^^^^^^^^

.. java:method:: public void recompute()
   :outertype: AdaptiveRandomNeighborhood

   Recomputes the neighbors

