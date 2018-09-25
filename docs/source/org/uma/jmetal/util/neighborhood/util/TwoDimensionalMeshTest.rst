.. java:import:: org.junit Rule

.. java:import:: org.junit Test

.. java:import:: org.junit.rules ExpectedException

.. java:import:: org.uma.jmetal.solution IntegerSolution

.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: java.util ArrayList

.. java:import:: java.util List

TwoDimensionalMeshTest
======================

.. java:package:: org.uma.jmetal.util.neighborhood.util
   :noindex:

.. java:type:: public class TwoDimensionalMeshTest

   Created by ajnebro on 21/5/15.

Fields
------
exception
^^^^^^^^^

.. java:field:: @Rule public ExpectedException exception
   :outertype: TwoDimensionalMeshTest

Methods
-------
shouldGetNeighborsReturnFourNeighborsCase1
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldGetNeighborsReturnFourNeighborsCase1()
   :outertype: TwoDimensionalMeshTest

   Case 1 Solution list: 0 1 2 3 4 5 6 7 8 The solution location is 4, the neighborhood is 1, 3, 5, 7

shouldGetNeighborsReturnFourNeighborsCase2
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldGetNeighborsReturnFourNeighborsCase2()
   :outertype: TwoDimensionalMeshTest

   Case 2 Solution list: 0 1 2 3 4 5 6 7 8 The solution location is 1, the neighborhood is 7, 0, 2, 4

shouldGetNeighborsReturnFourNeighborsCase3
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldGetNeighborsReturnFourNeighborsCase3()
   :outertype: TwoDimensionalMeshTest

   Case 3 Solution list: 0 1 2 3 4 5 6 7 8 The solution location is 0, the neighborhood is 1, 2, 3, 6

shouldGetNeighborsReturnFourNeighborsCase4
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldGetNeighborsReturnFourNeighborsCase4()
   :outertype: TwoDimensionalMeshTest

   Case 4 Solution list: 0 1 2 3 4 5 6 7 8 The solution location is 2, the neighborhood is 1, 0, 5, 8

shouldGetNeighborsReturnFourNeighborsCase5
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldGetNeighborsReturnFourNeighborsCase5()
   :outertype: TwoDimensionalMeshTest

   Case 5 Solution list: 0 1 2 3 4 5 6 7 8 The solution location is 2, the neighborhood is 2, 6, 7, 5

shouldGetNeighborsReturnFourNeighborsCase6
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldGetNeighborsReturnFourNeighborsCase6()
   :outertype: TwoDimensionalMeshTest

   Case 6 Solution list: 0 1 2 3 4 5 The solution location is 0, the neighborhood is 1, 3, 3, 2

shouldGetNeighborsReturnFourNeighborsCase7
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldGetNeighborsReturnFourNeighborsCase7()
   :outertype: TwoDimensionalMeshTest

   Case 7 Solution list: 0 1 2 3 4 5 The solution location is 3, the neighborhood is 0, 4, 5, 0

shouldGetNeighborsReturnFourNeighborsCase8
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldGetNeighborsReturnFourNeighborsCase8()
   :outertype: TwoDimensionalMeshTest

   Case 8 Solution list: 0 1 2 3 The solution location is 0, the neighborhood is 2, 1, 2, 1

shouldGetNeighborsWithANegativeSolutionIndexThrowAnException
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldGetNeighborsWithANegativeSolutionIndexThrowAnException()
   :outertype: TwoDimensionalMeshTest

shouldGetNeighborsWithANullListOfSolutionsThrowAnException
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldGetNeighborsWithANullListOfSolutionsThrowAnException()
   :outertype: TwoDimensionalMeshTest

shouldGetNeighborsWithASolutionIndexValueEqualToTheListSizeThrowAnException
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldGetNeighborsWithASolutionIndexValueEqualToTheListSizeThrowAnException()
   :outertype: TwoDimensionalMeshTest

shouldGetNeighborsWithASolutionIndexValueGreaterThanTheListSizeThrowAnException
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldGetNeighborsWithASolutionIndexValueGreaterThanTheListSizeThrowAnException()
   :outertype: TwoDimensionalMeshTest

shouldGetNeighborsWithAnEmptyListOfSolutionsThrowAnException
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldGetNeighborsWithAnEmptyListOfSolutionsThrowAnException()
   :outertype: TwoDimensionalMeshTest

