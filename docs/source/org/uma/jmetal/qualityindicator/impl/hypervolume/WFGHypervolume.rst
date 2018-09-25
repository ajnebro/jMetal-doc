.. java:import:: org.uma.jmetal.qualityindicator.impl Hypervolume

.. java:import:: org.uma.jmetal.qualityindicator.impl.hypervolume.util WfgHypervolumeFront

.. java:import:: org.uma.jmetal.qualityindicator.impl.hypervolume.util WfgHypervolumeVersion

.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util.comparator HypervolumeContributionComparator

.. java:import:: org.uma.jmetal.util.comparator ObjectiveComparator

.. java:import:: org.uma.jmetal.util.front Front

.. java:import:: org.uma.jmetal.util.point Point

.. java:import:: org.uma.jmetal.util.point.impl ArrayPoint

.. java:import:: org.uma.jmetal.util.solutionattribute.impl HypervolumeContributionAttribute

.. java:import:: java.io FileNotFoundException

.. java:import:: java.util Collections

.. java:import:: java.util List

WFGHypervolume
==============

.. java:package:: org.uma.jmetal.qualityindicator.impl.hypervolume
   :noindex:

.. java:type:: @SuppressWarnings public class WFGHypervolume<S extends Solution<?>> extends Hypervolume<S>

   Created by ajnebro on 2/2/15.

Constructors
------------
WFGHypervolume
^^^^^^^^^^^^^^

.. java:constructor:: public WFGHypervolume()
   :outertype: WFGHypervolume

   Default constructor

WFGHypervolume
^^^^^^^^^^^^^^

.. java:constructor:: public WFGHypervolume(String referenceParetoFrontFile) throws FileNotFoundException
   :outertype: WFGHypervolume

   Constructor

   :param referenceParetoFrontFile:
   :throws FileNotFoundException:

WFGHypervolume
^^^^^^^^^^^^^^

.. java:constructor:: public WFGHypervolume(Front referenceParetoFront)
   :outertype: WFGHypervolume

   Constructor

   :param referenceParetoFront:
   :throws FileNotFoundException:

Methods
-------
computeHypervolume
^^^^^^^^^^^^^^^^^^

.. java:method:: public double computeHypervolume(List<S> solutionList, Point referencePoint)
   :outertype: WFGHypervolume

computeHypervolumeContribution
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public List<S> computeHypervolumeContribution(List<S> solutionList, List<S> referenceFrontList)
   :outertype: WFGHypervolume

evaluate
^^^^^^^^

.. java:method:: @Override public Double evaluate(List<S> solutionList)
   :outertype: WFGHypervolume

get2DHV
^^^^^^^

.. java:method:: public double get2DHV(List<? extends Solution<?>> solutionSet)
   :outertype: WFGHypervolume

   Computes the HV of a solution list. REQUIRES: The problem is bi-objective REQUIRES: The setArchive is ordered in descending order by the second objective

getDescription
^^^^^^^^^^^^^^

.. java:method:: @Override public String getDescription()
   :outertype: WFGHypervolume

getOffset
^^^^^^^^^

.. java:method:: @Override public double getOffset()
   :outertype: WFGHypervolume

setOffset
^^^^^^^^^

.. java:method:: @Override public void setOffset(double offset)
   :outertype: WFGHypervolume

