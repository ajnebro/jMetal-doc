.. java:import:: java.util List

.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util JMetalException

NadirPoint
==========

.. java:package:: org.uma.jmetal.util.point.impl
   :noindex:

.. java:type:: @SuppressWarnings public class NadirPoint extends ArrayPoint

   Class representing a nadir point (minimization is assumed)

   :author: Antonio J.Nebro

Constructors
------------
NadirPoint
^^^^^^^^^^

.. java:constructor:: public NadirPoint(int dimension)
   :outertype: NadirPoint

Methods
-------
update
^^^^^^

.. java:method:: @Override public void update(double[] point)
   :outertype: NadirPoint

update
^^^^^^

.. java:method:: public void update(List<? extends Solution<?>> solutionList)
   :outertype: NadirPoint

