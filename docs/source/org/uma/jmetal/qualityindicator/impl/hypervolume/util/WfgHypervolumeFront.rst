.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: org.uma.jmetal.util.front.imp ArrayFront

.. java:import:: org.uma.jmetal.util.point Point

.. java:import:: java.util List

WfgHypervolumeFront
===================

.. java:package:: org.uma.jmetal.qualityindicator.impl.hypervolume.util
   :noindex:

.. java:type:: @SuppressWarnings public class WfgHypervolumeFront extends ArrayFront

   Created by ajnebro on 3/2/15.

Constructors
------------
WfgHypervolumeFront
^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public WfgHypervolumeFront()
   :outertype: WfgHypervolumeFront

WfgHypervolumeFront
^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public WfgHypervolumeFront(List<? extends Solution<?>> solutionList)
   :outertype: WfgHypervolumeFront

WfgHypervolumeFront
^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public WfgHypervolumeFront(int numberOfPoints, int dimensions)
   :outertype: WfgHypervolumeFront

Methods
-------
getNumberOfPoints
^^^^^^^^^^^^^^^^^

.. java:method:: @Override public int getNumberOfPoints()
   :outertype: WfgHypervolumeFront

getPoint
^^^^^^^^

.. java:method:: @Override public Point getPoint(int index)
   :outertype: WfgHypervolumeFront

setNumberOfPoints
^^^^^^^^^^^^^^^^^

.. java:method:: public void setNumberOfPoints(int numberOfPoints)
   :outertype: WfgHypervolumeFront

setPoint
^^^^^^^^

.. java:method:: @Override public void setPoint(int index, Point point)
   :outertype: WfgHypervolumeFront

