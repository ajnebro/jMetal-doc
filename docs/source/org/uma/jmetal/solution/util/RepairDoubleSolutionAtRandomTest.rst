.. java:import:: org.hamcrest Matchers

.. java:import:: org.junit Before

.. java:import:: org.junit Test

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: org.uma.jmetal.util.pseudorandom JMetalRandom

.. java:import:: org.uma.jmetal.util.pseudorandom.impl AuditableRandomGenerator

.. java:import:: java.util Random

RepairDoubleSolutionAtRandomTest
================================

.. java:package:: org.uma.jmetal.solution.util
   :noindex:

.. java:type:: public class RepairDoubleSolutionAtRandomTest

   :author: Antonio J. Nebro

Methods
-------
setup
^^^^^

.. java:method:: @Before public void setup()
   :outertype: RepairDoubleSolutionAtRandomTest

shouldJMetalRandomGeneratorNotBeUsedWhenCustomRandomGeneratorProvided
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldJMetalRandomGeneratorNotBeUsedWhenCustomRandomGeneratorProvided()
   :outertype: RepairDoubleSolutionAtRandomTest

shouldRRepairDoubleSolutionAtRandomAssignARandomValueIfValueIsGreaterThanTheUpperBound
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldRRepairDoubleSolutionAtRandomAssignARandomValueIfValueIsGreaterThanTheUpperBound()
   :outertype: RepairDoubleSolutionAtRandomTest

shouldRRepairDoubleSolutionAtRandomAssignARandomValueIfValueIsLessThanTheLowerBound
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldRRepairDoubleSolutionAtRandomAssignARandomValueIfValueIsLessThanTheLowerBound()
   :outertype: RepairDoubleSolutionAtRandomTest

shouldRRepairDoubleSolutionAtRandomRaiseAnExceptionIfTheBoundsAreIncorrect
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldRRepairDoubleSolutionAtRandomRaiseAnExceptionIfTheBoundsAreIncorrect()
   :outertype: RepairDoubleSolutionAtRandomTest

