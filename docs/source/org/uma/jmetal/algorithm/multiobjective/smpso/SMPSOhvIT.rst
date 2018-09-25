.. java:import:: org.junit Before

.. java:import:: org.junit Test

.. java:import:: org.uma.jmetal.algorithm Algorithm

.. java:import:: org.uma.jmetal.problem DoubleProblem

.. java:import:: org.uma.jmetal.problem.multiobjective.zdt ZDT4

.. java:import:: org.uma.jmetal.qualityindicator QualityIndicator

.. java:import:: org.uma.jmetal.qualityindicator.impl.hypervolume PISAHypervolume

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.util.archive BoundedArchive

.. java:import:: org.uma.jmetal.util.archive.impl HypervolumeArchive

.. java:import:: java.util List

SMPSOhvIT
=========

.. java:package:: org.uma.jmetal.algorithm.multiobjective.smpso
   :noindex:

.. java:type:: public class SMPSOhvIT

Methods
-------
setup
^^^^^

.. java:method:: @Before public void setup()
   :outertype: SMPSOhvIT

shouldTheAlgorithmReturnANumberOfSolutionsWhenSolvingASimpleProblem
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldTheAlgorithmReturnANumberOfSolutionsWhenSolvingASimpleProblem() throws Exception
   :outertype: SMPSOhvIT

shouldTheHypervolumeHaveAMininumValue
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldTheHypervolumeHaveAMininumValue() throws Exception
   :outertype: SMPSOhvIT

