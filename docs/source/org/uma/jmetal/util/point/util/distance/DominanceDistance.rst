.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: org.uma.jmetal.util.point Point

DominanceDistance
=================

.. java:package:: org.uma.jmetal.util.point.util.distance
   :noindex:

.. java:type:: public class DominanceDistance implements PointDistance

   Computes the distance between two points a y b according to the dominance relationship. Point a is supposed to be point of the Pareto front

   :author: Antonio J. Nebro

Methods
-------
compute
^^^^^^^

.. java:method:: @Override public double compute(Point a, Point b)
   :outertype: DominanceDistance

