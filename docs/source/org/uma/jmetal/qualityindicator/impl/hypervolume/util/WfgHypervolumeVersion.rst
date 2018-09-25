.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: org.uma.jmetal.util JMetalLogger

.. java:import:: org.uma.jmetal.util.front Front

.. java:import:: org.uma.jmetal.util.point Point

.. java:import:: org.uma.jmetal.util.point.impl ArrayPoint

.. java:import:: org.uma.jmetal.util.point.util.comparator PointComparator

.. java:import:: org.uma.jmetal.util.solutionattribute.impl HypervolumeContributionAttribute

.. java:import:: java.io IOException

.. java:import:: java.util Comparator

.. java:import:: java.util List

WfgHypervolumeVersion
=====================

.. java:package:: org.uma.jmetal.qualityindicator.impl.hypervolume.util
   :noindex:

.. java:type:: public class WfgHypervolumeVersion

   Created by ajnebro on 2/2/15.

Fields
------
OPT
^^^

.. java:field:: static final int OPT
   :outertype: WfgHypervolumeVersion

fs
^^

.. java:field::  WfgHypervolumeFront[] fs
   :outertype: WfgHypervolumeVersion

maximizing
^^^^^^^^^^

.. java:field::  boolean maximizing
   :outertype: WfgHypervolumeVersion

Constructors
------------
WfgHypervolumeVersion
^^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public WfgHypervolumeVersion(int dimension, int maxNumberOfPoints)
   :outertype: WfgHypervolumeVersion

WfgHypervolumeVersion
^^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public WfgHypervolumeVersion(int dimension, int maxNumberOfPoints, Point referencePoint)
   :outertype: WfgHypervolumeVersion

Methods
-------
dominates2way
^^^^^^^^^^^^^

.. java:method::  int dominates2way(Point p, Point q)
   :outertype: WfgHypervolumeVersion

get2DHV
^^^^^^^

.. java:method:: public double get2DHV(WfgHypervolumeFront front)
   :outertype: WfgHypervolumeVersion

getExclusiveHV
^^^^^^^^^^^^^^

.. java:method:: public double getExclusiveHV(WfgHypervolumeFront front, int point)
   :outertype: WfgHypervolumeVersion

getHV
^^^^^

.. java:method:: public double getHV(WfgHypervolumeFront front)
   :outertype: WfgHypervolumeVersion

getInclusiveHV
^^^^^^^^^^^^^^

.. java:method:: public double getInclusiveHV(Point point)
   :outertype: WfgHypervolumeVersion

getLessContributorHV
^^^^^^^^^^^^^^^^^^^^

.. java:method:: public int getLessContributorHV(List<Solution<?>> solutionList)
   :outertype: WfgHypervolumeVersion

main
^^^^

.. java:method:: public static void main(String[] args) throws IOException, JMetalException
   :outertype: WfgHypervolumeVersion

makeDominatedBit
^^^^^^^^^^^^^^^^

.. java:method:: public void makeDominatedBit(WfgHypervolumeFront front, int p)
   :outertype: WfgHypervolumeVersion

