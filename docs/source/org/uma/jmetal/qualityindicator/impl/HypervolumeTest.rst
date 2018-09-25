.. java:import:: org.junit Rule

.. java:import:: org.junit Test

.. java:import:: org.junit.rules ExpectedException

.. java:import:: org.uma.jmetal.qualityindicator.impl.hypervolume PISAHypervolume

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: org.uma.jmetal.util.front Front

.. java:import:: org.uma.jmetal.util.front.imp ArrayFront

HypervolumeTest
===============

.. java:package:: org.uma.jmetal.qualityindicator.impl
   :noindex:

.. java:type:: public class HypervolumeTest

   :author: Antonio J. Nebro

Fields
------
exception
^^^^^^^^^

.. java:field:: @Rule public ExpectedException exception
   :outertype: HypervolumeTest

Methods
-------
shouldExecuteRaiseAnExceptionIfTheFrontApproximationIsNull
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldExecuteRaiseAnExceptionIfTheFrontApproximationIsNull()
   :outertype: HypervolumeTest

shouldExecuteRaiseAnExceptionIfTheParetoFrontIsNull
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldExecuteRaiseAnExceptionIfTheParetoFrontIsNull()
   :outertype: HypervolumeTest

