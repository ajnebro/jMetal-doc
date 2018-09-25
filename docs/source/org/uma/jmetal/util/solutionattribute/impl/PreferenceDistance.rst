.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util.comparator ObjectiveComparator

.. java:import:: org.uma.jmetal.util.pseudorandom JMetalRandom

.. java:import:: org.uma.jmetal.util.solutionattribute DensityEstimator

.. java:import:: java.util ArrayList

.. java:import:: java.util Collections

.. java:import:: java.util LinkedList

.. java:import:: java.util List

PreferenceDistance
==================

.. java:package:: org.uma.jmetal.util.solutionattribute.impl
   :noindex:

.. java:type:: public class PreferenceDistance<S extends Solution<?>> extends GenericSolutionAttribute<S, Double> implements DensityEstimator<S>

Constructors
------------
PreferenceDistance
^^^^^^^^^^^^^^^^^^

.. java:constructor:: public PreferenceDistance(List<Double> interestPoint, double epsilon)
   :outertype: PreferenceDistance

Methods
-------
computeDensityEstimator
^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public void computeDensityEstimator(List<S> solutionList)
   :outertype: PreferenceDistance

epsilonClean
^^^^^^^^^^^^

.. java:method:: public List<S> epsilonClean(List<S> solutionList)
   :outertype: PreferenceDistance

getSize
^^^^^^^

.. java:method:: public int getSize()
   :outertype: PreferenceDistance

updatePointOfInterest
^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public void updatePointOfInterest(List<Double> newInterestPoint)
   :outertype: PreferenceDistance

