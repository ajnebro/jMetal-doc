.. java:import:: java.util List

.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util JMetalException

IdealPoint
==========

.. java:package:: org.uma.jmetal.util.point.impl
   :noindex:

.. java:type:: @SuppressWarnings public class IdealPoint extends ArrayPoint

   d Class representing an ideal point (minimization is assumed)

   :author: Antonio J.Nebro

Constructors
------------
IdealPoint
^^^^^^^^^^

.. java:constructor:: public IdealPoint(int dimension)
   :outertype: IdealPoint

Methods
-------
update
^^^^^^

.. java:method:: @Override public void update(double[] point)
   :outertype: IdealPoint

update
^^^^^^

.. java:method:: public void update(List<? extends Solution<?>> solutionList)
   :outertype: IdealPoint

