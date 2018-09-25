.. java:import:: org.uma.jmetal.qualityindicator.impl Hypervolume

.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util SolutionListUtils

.. java:import:: org.uma.jmetal.util.comparator HypervolumeContributionComparator

.. java:import:: java.util Collections

.. java:import:: java.util Comparator

HypervolumeArchive
==================

.. java:package:: org.uma.jmetal.util.archive.impl
   :noindex:

.. java:type:: @SuppressWarnings public class HypervolumeArchive<S extends Solution<?>> extends AbstractBoundedArchive<S>

   Created by Antonio J. Nebro on 24/09/14.

Fields
------
hypervolume
^^^^^^^^^^^

.. java:field::  Hypervolume<S> hypervolume
   :outertype: HypervolumeArchive

Constructors
------------
HypervolumeArchive
^^^^^^^^^^^^^^^^^^

.. java:constructor:: public HypervolumeArchive(int maxSize, Hypervolume<S> hypervolume)
   :outertype: HypervolumeArchive

Methods
-------
computeDensityEstimator
^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public void computeDensityEstimator()
   :outertype: HypervolumeArchive

getComparator
^^^^^^^^^^^^^

.. java:method:: @Override public Comparator<S> getComparator()
   :outertype: HypervolumeArchive

prune
^^^^^

.. java:method:: @Override public void prune()
   :outertype: HypervolumeArchive

sortByDensityEstimator
^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public void sortByDensityEstimator()
   :outertype: HypervolumeArchive

