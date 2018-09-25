.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: org.uma.jmetal.util JMetalLogger

Transformations
===============

.. java:package:: org.uma.jmetal.problem.multiobjective.wfg
   :noindex:

.. java:type:: public class Transformations

   Class implementing the basics transformations for wfg

Methods
-------
bFlat
^^^^^

.. java:method:: public float bFlat(float y, float A, float B, float C)
   :outertype: Transformations

   bFlat transformation

bParam
^^^^^^

.. java:method:: public float bParam(float y, float u, float A, float B, float C)
   :outertype: Transformations

   bParam transformation

bPoly
^^^^^

.. java:method:: public float bPoly(float y, float alpha) throws JMetalException
   :outertype: Transformations

   bPoly transformation

   :throws org.uma.jmetal.util.JMetalException:

correctTo01
^^^^^^^^^^^

.. java:method::  float correctTo01(float a)
   :outertype: Transformations

rNonsep
^^^^^^^

.. java:method:: public float rNonsep(float[] y, int A)
   :outertype: Transformations

   rNonsep transformation

rSum
^^^^

.. java:method:: public float rSum(float[] y, float[] w)
   :outertype: Transformations

   rSum transformation

sDecept
^^^^^^^

.. java:method:: public float sDecept(float y, float A, float B, float C)
   :outertype: Transformations

   sDecept transformation

sLinear
^^^^^^^

.. java:method:: public float sLinear(float y, float A)
   :outertype: Transformations

   sLinear transformation

sMulti
^^^^^^

.. java:method:: public float sMulti(float y, int A, int B, float C)
   :outertype: Transformations

   sMulti transformation

