.. java:import:: org.junit Rule

.. java:import:: org.junit Test

.. java:import:: org.junit.rules ExpectedException

.. java:import:: org.springframework.test.util ReflectionTestUtils

.. java:import:: org.uma.jmetal.solution BinarySolution

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: java.util ArrayList

.. java:import:: java.util Comparator

.. java:import:: java.util List

TournamentSelectionTest
=======================

.. java:package:: org.uma.jmetal.operator.impl.selection
   :noindex:

.. java:type:: public class TournamentSelectionTest

   Created by ajnebro on 3/5/15.

Fields
------
exception
^^^^^^^^^

.. java:field:: @Rule public ExpectedException exception
   :outertype: TournamentSelectionTest

Methods
-------
shouldConstructorAssignTheCorrectValueSToTheNumberOfTournamentsAndTheComparator
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldConstructorAssignTheCorrectValueSToTheNumberOfTournamentsAndTheComparator()
   :outertype: TournamentSelectionTest

shouldConstructorAssignTheCorrectValueToTheNumberOfTournaments
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldConstructorAssignTheCorrectValueToTheNumberOfTournaments()
   :outertype: TournamentSelectionTest

shouldExecuteRaiseAnExceptionIfTheSolutionListIsEmpty
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldExecuteRaiseAnExceptionIfTheSolutionListIsEmpty()
   :outertype: TournamentSelectionTest

shouldExecuteRaiseAnExceptionIfTheSolutionListIsNull
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldExecuteRaiseAnExceptionIfTheSolutionListIsNull()
   :outertype: TournamentSelectionTest

shouldExecuteReturnAnElementIfTheListHasOneElement
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldExecuteReturnAnElementIfTheListHasOneElement()
   :outertype: TournamentSelectionTest

