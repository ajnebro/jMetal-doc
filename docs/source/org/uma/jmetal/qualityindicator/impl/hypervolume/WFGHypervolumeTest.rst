.. java:import:: org.junit Before

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

.. java:import:: java.util Arrays

.. java:import:: java.util List

WFGHypervolumeTest
==================

.. java:package:: org.uma.jmetal.qualityindicator.impl.hypervolume
   :noindex:

.. java:type:: public class WFGHypervolumeTest

   Created by ajnebro on 17/12/15.

Methods
-------
setup
^^^^^

.. java:method:: @Before public void setup()
   :outertype: WFGHypervolumeTest

shouldEvaluateWorkProperlyCase1
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldEvaluateWorkProperlyCase1() throws FileNotFoundException
   :outertype: WFGHypervolumeTest

   CASE 1: solution set -> front composed of the points [0.25, 0.75] and [0.75, 0.25]. Reference point: [1.0, 1.0]

shouldEvaluateWorkProperlyCase2
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldEvaluateWorkProperlyCase2() throws FileNotFoundException
   :outertype: WFGHypervolumeTest

   CASE 2: solution set -> front composed of the points [0.25, 0.75], [0.75, 0.25] and [0.5, 0.5]. Reference point: [1.0, 1.0]

shouldEvaluateWorkProperlyCase3
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldEvaluateWorkProperlyCase3() throws FileNotFoundException
   :outertype: WFGHypervolumeTest

   CASE 3: solution set -> front composed of the points [0.25, 0.75], [0.75, 0.25] and [0.5, 0.5]. Reference point: [1.5, 1.5]

shouldEvaluateWorkProperlyCase4
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldEvaluateWorkProperlyCase4() throws FileNotFoundException
   :outertype: WFGHypervolumeTest

   CASE 4: solution set -> front obtained from the ZDT1.rf file. Reference point: [1.0, 1,0]

   :throws FileNotFoundException:

simpleTest
^^^^^^^^^^

.. java:method:: @Test public void simpleTest()
   :outertype: WFGHypervolumeTest

