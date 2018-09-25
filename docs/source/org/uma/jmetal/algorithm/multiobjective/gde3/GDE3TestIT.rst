.. java:import:: org.junit Test

.. java:import:: org.uma.jmetal.algorithm Algorithm

.. java:import:: org.uma.jmetal.problem DoubleProblem

.. java:import:: org.uma.jmetal.problem.multiobjective.zdt ZDT1

.. java:import:: org.uma.jmetal.qualityindicator QualityIndicator

.. java:import:: org.uma.jmetal.qualityindicator.impl.hypervolume PISAHypervolume

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.util AlgorithmRunner

.. java:import:: org.uma.jmetal.util.pseudorandom JMetalRandom

.. java:import:: java.util List

GDE3TestIT
==========

.. java:package:: org.uma.jmetal.algorithm.multiobjective.gde3
   :noindex:

.. java:type:: public class GDE3TestIT

   Created by ajnebro on 3/11/15.

Fields
------
algorithm
^^^^^^^^^

.. java:field::  Algorithm<List<DoubleSolution>> algorithm
   :outertype: GDE3TestIT

Methods
-------
shouldTheAlgorithmReturnANumberOfSolutionsWhenSolvingASimpleProblem
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldTheAlgorithmReturnANumberOfSolutionsWhenSolvingASimpleProblem() throws Exception
   :outertype: GDE3TestIT

shouldTheHypervolumeHaveAMininumValue
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldTheHypervolumeHaveAMininumValue() throws Exception
   :outertype: GDE3TestIT

