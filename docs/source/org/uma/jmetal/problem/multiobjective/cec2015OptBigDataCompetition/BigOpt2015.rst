.. java:import:: org.uma.jmetal.problem.impl AbstractDoubleProblem

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: java.io BufferedReader

.. java:import:: java.io IOException

.. java:import:: java.io InputStream

.. java:import:: java.io InputStreamReader

.. java:import:: java.util ArrayList

.. java:import:: java.util List

.. java:import:: java.util StringTokenizer

BigOpt2015
==========

.. java:package:: org.uma.jmetal.problem.multiobjective.cec2015OptBigDataCompetition
   :noindex:

.. java:type:: @SuppressWarnings public class BigOpt2015 extends AbstractDoubleProblem

   Created by ajnebro on 14/1/15.

Fields
------
dTypeG
^^^^^^

.. java:field::  int dTypeG
   :outertype: BigOpt2015

f1max
^^^^^

.. java:field::  double f1max
   :outertype: BigOpt2015

f1min
^^^^^

.. java:field::  double f1min
   :outertype: BigOpt2015

f2max
^^^^^

.. java:field::  double f2max
   :outertype: BigOpt2015

f2min
^^^^^

.. java:field::  double f2min
   :outertype: BigOpt2015

scaling
^^^^^^^

.. java:field::  boolean scaling
   :outertype: BigOpt2015

Constructors
------------
BigOpt2015
^^^^^^^^^^

.. java:constructor:: public BigOpt2015(String instanceName)
   :outertype: BigOpt2015

   Constructor

Methods
-------
correlation
^^^^^^^^^^^

.. java:method::  List<List<Double>> correlation(List<List<Double>> list1, List<List<Double>> list2)
   :outertype: BigOpt2015

diagonal1
^^^^^^^^^

.. java:method::  double diagonal1(List<List<Double>> list)
   :outertype: BigOpt2015

diagonal2
^^^^^^^^^

.. java:method::  double diagonal2(List<List<Double>> list)
   :outertype: BigOpt2015

evaluate
^^^^^^^^

.. java:method:: @Override public void evaluate(DoubleSolution solution)
   :outertype: BigOpt2015

   Evaluate() method

multiplyWithOutAMP
^^^^^^^^^^^^^^^^^^

.. java:method::  List<List<Double>> multiplyWithOutAMP(List<List<Double>> list1, List<List<Double>> list2)
   :outertype: BigOpt2015

newMeanStandardDeviation
^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method::  List<Double> newMeanStandardDeviation(List<Double> list)
   :outertype: BigOpt2015

vectorCorrelation
^^^^^^^^^^^^^^^^^

.. java:method::  double vectorCorrelation(List<Double> list1, List<Double> list2)
   :outertype: BigOpt2015

