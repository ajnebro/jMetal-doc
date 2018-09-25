.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util.archivewithreferencepoint ArchiveWithReferencePoint

.. java:import:: org.uma.jmetal.util.comparator CrowdingDistanceComparator

.. java:import:: org.uma.jmetal.util.solutionattribute DensityEstimator

.. java:import:: org.uma.jmetal.util.solutionattribute.impl CrowdingDistance

.. java:import:: java.util Collections

.. java:import:: java.util Comparator

.. java:import:: java.util List

CrowdingDistanceArchiveWithReferencePoint
=========================================

.. java:package:: org.uma.jmetal.util.archivewithreferencepoint.impl
   :noindex:

.. java:type:: public class CrowdingDistanceArchiveWithReferencePoint<S extends Solution<?>> extends ArchiveWithReferencePoint<S>

   Class representing a \ :java:ref:`ArchiveWithReferencePoint`\  archive using a crowding distance based density estimator

   :author: Antonio J. Nebro

Constructors
------------
CrowdingDistanceArchiveWithReferencePoint
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public CrowdingDistanceArchiveWithReferencePoint(int maxSize, List<Double> refPointDM)
   :outertype: CrowdingDistanceArchiveWithReferencePoint

Methods
-------
computeDensityEstimator
^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public void computeDensityEstimator()
   :outertype: CrowdingDistanceArchiveWithReferencePoint

getComparator
^^^^^^^^^^^^^

.. java:method:: @Override public Comparator<S> getComparator()
   :outertype: CrowdingDistanceArchiveWithReferencePoint

sortByDensityEstimator
^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public void sortByDensityEstimator()
   :outertype: CrowdingDistanceArchiveWithReferencePoint

