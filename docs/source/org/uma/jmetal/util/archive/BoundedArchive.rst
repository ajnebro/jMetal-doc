.. java:import:: java.util Comparator

BoundedArchive
==============

.. java:package:: org.uma.jmetal.util.archive
   :noindex:

.. java:type:: public interface BoundedArchive<S> extends Archive<S>

   Interface representing a bounded archive of solutions

   :author: Antonio J. Nebro

Methods
-------
computeDensityEstimator
^^^^^^^^^^^^^^^^^^^^^^^

.. java:method::  void computeDensityEstimator()
   :outertype: BoundedArchive

getComparator
^^^^^^^^^^^^^

.. java:method::  Comparator<S> getComparator()
   :outertype: BoundedArchive

getMaxSize
^^^^^^^^^^

.. java:method::  int getMaxSize()
   :outertype: BoundedArchive

sortByDensityEstimator
^^^^^^^^^^^^^^^^^^^^^^

.. java:method::  void sortByDensityEstimator()
   :outertype: BoundedArchive

