.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: org.uma.jmetal.util.neighborhood Neighborhood

.. java:import:: java.util ArrayList

.. java:import:: java.util List

TwoDimensionalMesh
==================

.. java:package:: org.uma.jmetal.util.neighborhood.util
   :noindex:

.. java:type:: @SuppressWarnings public class TwoDimensionalMesh<S> implements Neighborhood<S>

   Class defining a bi-dimensional mesh.

Constructors
------------
TwoDimensionalMesh
^^^^^^^^^^^^^^^^^^

.. java:constructor:: public TwoDimensionalMesh(int rows, int columns, int[][] neighborhood)
   :outertype: TwoDimensionalMesh

   Constructor. Defines a neighborhood for list of solutions

Methods
-------
getNeighbors
^^^^^^^^^^^^

.. java:method:: public List<S> getNeighbors(List<S> solutionList, int solutionPosition)
   :outertype: TwoDimensionalMesh

   Returns the north,south, east, and west solutions of a given solution

   :param solutionList: the solution set from where the neighbors are taken
   :param solutionPosition: Represents the position of the solution

