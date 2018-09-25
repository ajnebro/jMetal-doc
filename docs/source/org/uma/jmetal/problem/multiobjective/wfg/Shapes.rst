Shapes
======

.. java:package:: org.uma.jmetal.problem.multiobjective.wfg
   :noindex:

.. java:type:: public class Shapes

   Class implementing shape functions for wfg benchmark Reference: Simon Huband, Luigi Barone, Lyndon While, Phil Hingston A Scalable Multi-objective Test Problem Toolkit. Evolutionary Multi-Criterion Optimization: Third International Conference, EMO 2005. Proceedings, volume 3410 of Lecture Notes in Computer Science

Methods
-------
concave
^^^^^^^

.. java:method:: public float concave(float[] x, int m)
   :outertype: Shapes

   Calculate a concave shape

convex
^^^^^^

.. java:method:: public float convex(float[] x, int m)
   :outertype: Shapes

   Calculate a convex shape

disc
^^^^

.. java:method:: public float disc(float[] x, int A, float alpha, float beta)
   :outertype: Shapes

   Calculate a disc shape

linear
^^^^^^

.. java:method:: public float linear(float[] x, int m)
   :outertype: Shapes

   Calculate a linear shape

mixed
^^^^^

.. java:method:: public float mixed(float[] x, int A, float alpha)
   :outertype: Shapes

   Calculate a mixed shape

