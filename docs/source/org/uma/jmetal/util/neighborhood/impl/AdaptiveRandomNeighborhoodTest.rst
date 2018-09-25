.. java:import:: org.junit Rule

.. java:import:: org.junit Test

.. java:import:: org.junit.rules ExpectedException

.. java:import:: org.springframework.test.util ReflectionTestUtils

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.solution IntegerSolution

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: org.uma.jmetal.util.pseudorandom BoundedRandomGenerator

.. java:import:: org.uma.jmetal.util.pseudorandom JMetalRandom

.. java:import:: org.uma.jmetal.util.pseudorandom.impl AuditableRandomGenerator

.. java:import:: java.util ArrayList

.. java:import:: java.util List

.. java:import:: java.util Random

AdaptiveRandomNeighborhoodTest
==============================

.. java:package:: org.uma.jmetal.util.neighborhood.impl
   :noindex:

.. java:type:: public class AdaptiveRandomNeighborhoodTest

   :author: Antonio J. Nebro

Fields
------
exception
^^^^^^^^^

.. java:field:: @Rule public ExpectedException exception
   :outertype: AdaptiveRandomNeighborhoodTest

Methods
-------
shouldConstructorCreateAnInstanceIfTheParamtersAreValid
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldConstructorCreateAnInstanceIfTheParamtersAreValid()
   :outertype: AdaptiveRandomNeighborhoodTest

shouldConstructorThrowAnExceptionWhenTheNumberOfNeighboursIsEqualThanTheListSize
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldConstructorThrowAnExceptionWhenTheNumberOfNeighboursIsEqualThanTheListSize()
   :outertype: AdaptiveRandomNeighborhoodTest

shouldConstructorThrowAnExceptionWhenTheNumberOfNeighboursIsGreaterThanTheListSize
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldConstructorThrowAnExceptionWhenTheNumberOfNeighboursIsGreaterThanTheListSize()
   :outertype: AdaptiveRandomNeighborhoodTest

shouldConstructorThrowAnExceptionWhenTheNumberOfNeighboursIsNegative
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldConstructorThrowAnExceptionWhenTheNumberOfNeighboursIsNegative()
   :outertype: AdaptiveRandomNeighborhoodTest

shouldGetNeighborsReturnThreeNeighborsPlusTheCurrentSolution
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldGetNeighborsReturnThreeNeighborsPlusTheCurrentSolution()
   :outertype: AdaptiveRandomNeighborhoodTest

   Case 1 Solution list size: 3 Number of neighbors: 1 Neighbors: - solution 0: 0, 2 - solution 1: 1, 0 - solution 2: 2, 0

shouldGetNeighborsReturnTwoNeighborsPlusTheCurrentSolution
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldGetNeighborsReturnTwoNeighborsPlusTheCurrentSolution()
   :outertype: AdaptiveRandomNeighborhoodTest

   Case 1 Solution list size: 4 Number of neighbors: 2

shouldGetNeighborsThrowAnExceptionIfTheListSizeIsNotCorrect
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldGetNeighborsThrowAnExceptionIfTheListSizeIsNotCorrect()
   :outertype: AdaptiveRandomNeighborhoodTest

shouldGetNeighborsWithANegativeSolutionIndexThrowAnException
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldGetNeighborsWithANegativeSolutionIndexThrowAnException()
   :outertype: AdaptiveRandomNeighborhoodTest

shouldGetNeighborsWithANullListOfSolutionsThrowAnException
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldGetNeighborsWithANullListOfSolutionsThrowAnException()
   :outertype: AdaptiveRandomNeighborhoodTest

shouldGetNeighborsWithATooBigSolutionIndexThrowAnException
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldGetNeighborsWithATooBigSolutionIndexThrowAnException()
   :outertype: AdaptiveRandomNeighborhoodTest

shouldJMetalRandomGeneratorNotBeUsedWhenCustomRandomGeneratorProvided
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldJMetalRandomGeneratorNotBeUsedWhenCustomRandomGeneratorProvided()
   :outertype: AdaptiveRandomNeighborhoodTest

