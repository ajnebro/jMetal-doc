.. java:import:: org.uma.jmetal.qualityindicator.impl Hypervolume

.. java:import:: org.uma.jmetal.qualityindicator.impl.hypervolume PISAHypervolume

.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util.archivewithreferencepoint ArchiveWithReferencePoint

.. java:import:: org.uma.jmetal.util.comparator HypervolumeContributionComparator

.. java:import:: java.util Collections

.. java:import:: java.util Comparator

.. java:import:: java.util List

HypervolumeArchiveWithReferencePoint
====================================

.. java:package:: org.uma.jmetal.util.archivewithreferencepoint.impl
   :noindex:

.. java:type:: public class HypervolumeArchiveWithReferencePoint<S extends Solution<?>> extends ArchiveWithReferencePoint<S>

   Class representing a \ :java:ref:`ArchiveWithReferencePoint`\  archive using a hypervolume contribution based density estimator.

   :author: Antonio J. Nebro

Constructors
------------
HypervolumeArchiveWithReferencePoint
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public HypervolumeArchiveWithReferencePoint(int maxSize, List<Double> refPointDM)
   :outertype: HypervolumeArchiveWithReferencePoint

Methods
-------
computeDensityEstimator
^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public void computeDensityEstimator()
   :outertype: HypervolumeArchiveWithReferencePoint

getComparator
^^^^^^^^^^^^^

.. java:method:: @Override public Comparator<S> getComparator()
   :outertype: HypervolumeArchiveWithReferencePoint

sortByDensityEstimator
^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public void sortByDensityEstimator()
   :outertype: HypervolumeArchiveWithReferencePoint

