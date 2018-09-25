.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util SolutionListUtils

.. java:import:: org.uma.jmetal.util.comparator CrowdingDistanceComparator

.. java:import:: org.uma.jmetal.util.solutionattribute DensityEstimator

.. java:import:: org.uma.jmetal.util.solutionattribute.impl CrowdingDistance

.. java:import:: java.util Collections

.. java:import:: java.util Comparator

CrowdingDistanceArchive
=======================

.. java:package:: org.uma.jmetal.util.archive.impl
   :noindex:

.. java:type:: @SuppressWarnings public class CrowdingDistanceArchive<S extends Solution<?>> extends AbstractBoundedArchive<S>

   Created by Antonio J. Nebro on 24/09/14. Modified by Juanjo on 07/04/2015

Constructors
------------
CrowdingDistanceArchive
^^^^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public CrowdingDistanceArchive(int maxSize)
   :outertype: CrowdingDistanceArchive

Methods
-------
computeDensityEstimator
^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public void computeDensityEstimator()
   :outertype: CrowdingDistanceArchive

getComparator
^^^^^^^^^^^^^

.. java:method:: @Override public Comparator<S> getComparator()
   :outertype: CrowdingDistanceArchive

prune
^^^^^

.. java:method:: @Override public void prune()
   :outertype: CrowdingDistanceArchive

sortByDensityEstimator
^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public void sortByDensityEstimator()
   :outertype: CrowdingDistanceArchive

