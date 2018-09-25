.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util.comparator ObjectiveComparator

.. java:import:: org.uma.jmetal.util.solutionattribute DensityEstimator

.. java:import:: java.util ArrayList

.. java:import:: java.util Collections

.. java:import:: java.util List

CrowdingDistance
================

.. java:package:: org.uma.jmetal.util.solutionattribute.impl
   :noindex:

.. java:type:: @SuppressWarnings public class CrowdingDistance<S extends Solution<?>> extends GenericSolutionAttribute<S, Double> implements DensityEstimator<S>

   This class implements the crowding distance

   :author: Antonio J. Nebro

Methods
-------
computeDensityEstimator
^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public void computeDensityEstimator(List<S> solutionList)
   :outertype: CrowdingDistance

   Assigns crowding distances to all solutions in a \ ``SolutionSet``\ .

   :param solutionList: The \ ``SolutionSet``\ .
   :throws org.uma.jmetal.util.JMetalException:

getAttributeIdentifier
^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public Object getAttributeIdentifier()
   :outertype: CrowdingDistance

