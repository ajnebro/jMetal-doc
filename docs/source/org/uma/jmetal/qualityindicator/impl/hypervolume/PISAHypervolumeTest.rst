.. java:import:: org.junit Test

.. java:import:: org.uma.jmetal.problem DoubleProblem

.. java:import:: org.uma.jmetal.problem.impl AbstractDoubleProblem

.. java:import:: org.uma.jmetal.qualityindicator.impl Hypervolume

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.solution.impl DefaultDoubleSolution

.. java:import:: org.uma.jmetal.util.front Front

.. java:import:: org.uma.jmetal.util.front.imp ArrayFront

.. java:import:: org.uma.jmetal.util.point.impl ArrayPoint

.. java:import:: java.io FileNotFoundException

.. java:import:: java.util ArrayList

.. java:import:: java.util List

PISAHypervolumeTest
===================

.. java:package:: org.uma.jmetal.qualityindicator.impl.hypervolume
   :noindex:

.. java:type:: public class PISAHypervolumeTest

Methods
-------
shouldEvaluateWorkProperlyCase1
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldEvaluateWorkProperlyCase1() throws FileNotFoundException
   :outertype: PISAHypervolumeTest

   CASE 1: solution set -> front obtained from the ZDT1.rf file. Reference front: [0,1], [1,0]

   :throws FileNotFoundException:

