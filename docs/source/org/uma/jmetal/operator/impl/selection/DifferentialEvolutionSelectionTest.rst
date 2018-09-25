.. java:import:: org.junit Rule

.. java:import:: org.junit Test

.. java:import:: org.junit.rules ExpectedException

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: org.uma.jmetal.util.pseudorandom JMetalRandom

.. java:import:: org.uma.jmetal.util.pseudorandom.impl AuditableRandomGenerator

.. java:import:: java.util Arrays

.. java:import:: java.util Collections

.. java:import:: java.util List

.. java:import:: java.util Random

DifferentialEvolutionSelectionTest
==================================

.. java:package:: org.uma.jmetal.operator.impl.selection
   :noindex:

.. java:type:: public class DifferentialEvolutionSelectionTest

   Created by ajnebro on 3/5/15.

Fields
------
exception
^^^^^^^^^

.. java:field:: @Rule public ExpectedException exception
   :outertype: DifferentialEvolutionSelectionTest

Methods
-------
shouldExecuteRaiseAnExceptionIfTheIndexIsHigherThanTheSolutionListLength
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldExecuteRaiseAnExceptionIfTheIndexIsHigherThanTheSolutionListLength()
   :outertype: DifferentialEvolutionSelectionTest

shouldExecuteRaiseAnExceptionIfTheIndexIsNegative
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldExecuteRaiseAnExceptionIfTheIndexIsNegative()
   :outertype: DifferentialEvolutionSelectionTest

shouldExecuteRaiseAnExceptionIfTheIndexIsNotIndicated
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldExecuteRaiseAnExceptionIfTheIndexIsNotIndicated()
   :outertype: DifferentialEvolutionSelectionTest

shouldExecuteRaiseAnExceptionIfTheListOfSolutionsHasOneSolution
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldExecuteRaiseAnExceptionIfTheListOfSolutionsHasOneSolution()
   :outertype: DifferentialEvolutionSelectionTest

shouldExecuteRaiseAnExceptionIfTheListOfSolutionsIsEmpty
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldExecuteRaiseAnExceptionIfTheListOfSolutionsIsEmpty()
   :outertype: DifferentialEvolutionSelectionTest

shouldExecuteRaiseAnExceptionIfTheListOfSolutionsIsNull
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldExecuteRaiseAnExceptionIfTheListOfSolutionsIsNull()
   :outertype: DifferentialEvolutionSelectionTest

shouldExecuteReturnThreeDifferentSolutionsIfTheListHasFourElements
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldExecuteReturnThreeDifferentSolutionsIfTheListHasFourElements()
   :outertype: DifferentialEvolutionSelectionTest

shouldJMetalRandomGeneratorNotBeUsedWhenCustomRandomGeneratorProvided
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldJMetalRandomGeneratorNotBeUsedWhenCustomRandomGeneratorProvided()
   :outertype: DifferentialEvolutionSelectionTest

