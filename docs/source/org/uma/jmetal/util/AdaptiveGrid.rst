.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util.pseudorandom BoundedRandomGenerator

.. java:import:: org.uma.jmetal.util.pseudorandom JMetalRandom

.. java:import:: java.util List

AdaptiveGrid
============

.. java:package:: org.uma.jmetal.util
   :noindex:

.. java:type:: public class AdaptiveGrid<S extends Solution<?>>

   This class defines an adaptive grid over a list of solutions as the one used by algorithm PAES.

   :author: Antonio J. Nebro, Juan J. Durillo

Constructors
------------
AdaptiveGrid
^^^^^^^^^^^^

.. java:constructor:: public AdaptiveGrid(int bisections, int objectives)
   :outertype: AdaptiveGrid

   Constructor. Creates an instance of AdaptiveGrid.

   :param bisections: Number of bi-divisions of the objective space.
   :param objectives: Number of numberOfObjectives of the problem.

Methods
-------
addSolution
^^^^^^^^^^^

.. java:method:: public void addSolution(int location)
   :outertype: AdaptiveGrid

   Increases the number of solutions into a specific hypercube.

   :param location: Number of hypercube.

calculateOccupied
^^^^^^^^^^^^^^^^^

.. java:method:: public void calculateOccupied()
   :outertype: AdaptiveGrid

   Calculates the number of hypercubes having one or more solutions. return the number of hypercubes with more than zero solutions.

getAverageOccupation
^^^^^^^^^^^^^^^^^^^^

.. java:method:: public double getAverageOccupation()
   :outertype: AdaptiveGrid

   Return the average number of solutions in the occupied hypercubes

getBisections
^^^^^^^^^^^^^

.. java:method:: public int getBisections()
   :outertype: AdaptiveGrid

   Returns the number of bi-divisions performed in each objective.

   :return: the number of bi-divisions.

getHypercubes
^^^^^^^^^^^^^

.. java:method:: public int[] getHypercubes()
   :outertype: AdaptiveGrid

getLocationDensity
^^^^^^^^^^^^^^^^^^

.. java:method:: public int getLocationDensity(int location)
   :outertype: AdaptiveGrid

   Returns the number of solutions into a specific hypercube.

   :param location: Number of the hypercube.
   :return: The number of solutions into a specific hypercube.

getMostPopulatedHypercube
^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public int getMostPopulatedHypercube()
   :outertype: AdaptiveGrid

   Returns the value of the most populated hypercube.

   :return: The hypercube with the maximum number of solutions.

location
^^^^^^^^

.. java:method:: public int location(S solution)
   :outertype: AdaptiveGrid

   Calculates the hypercube of a solution

   :param solution: The \ ``Solution``\ .

occupiedHypercubes
^^^^^^^^^^^^^^^^^^

.. java:method:: public int occupiedHypercubes()
   :outertype: AdaptiveGrid

   Returns the number of hypercubes with more than zero solutions.

   :return: the number of hypercubes with more than zero solutions.

randomOccupiedHypercube
^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public int randomOccupiedHypercube()
   :outertype: AdaptiveGrid

   Returns a random hypercube that has more than zero solutions.

   :return: The hypercube.

randomOccupiedHypercube
^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public int randomOccupiedHypercube(BoundedRandomGenerator<Integer> randomGenerator)
   :outertype: AdaptiveGrid

   Returns a random hypercube that has more than zero solutions.

   :param randomGenerator: the \ :java:ref:`BoundedRandomGenerator`\  to use for selecting the hypercube
   :return: The hypercube.

removeSolution
^^^^^^^^^^^^^^

.. java:method:: public void removeSolution(int location)
   :outertype: AdaptiveGrid

   Decreases the number of solutions into a specific hypercube.

   :param location: Number of hypercube.

rouletteWheel
^^^^^^^^^^^^^

.. java:method:: public int rouletteWheel()
   :outertype: AdaptiveGrid

   Returns a random hypercube using a rouleteWheel method.

   :return: the number of the selected hypercube.

rouletteWheel
^^^^^^^^^^^^^

.. java:method:: public int rouletteWheel(BoundedRandomGenerator<Double> randomGenerator)
   :outertype: AdaptiveGrid

   Returns a random hypercube using a rouleteWheel method.

   :param randomGenerator: the \ :java:ref:`BoundedRandomGenerator`\  to use for the roulette
   :return: the number of the selected hypercube.

toString
^^^^^^^^

.. java:method:: public String toString()
   :outertype: AdaptiveGrid

   Returns a String representing the grid.

   :return: The String.

updateGrid
^^^^^^^^^^

.. java:method:: public void updateGrid(List<S> solutionList)
   :outertype: AdaptiveGrid

   Updates the grid limits and the grid content adding the solutions contained in a specific \ ``solutionList``\ .

   :param solutionList: The \ ``solutionList``\ .

updateGrid
^^^^^^^^^^

.. java:method:: public void updateGrid(S solution, List<S> solutionSet)
   :outertype: AdaptiveGrid

   Updates the grid limits and the grid content adding a new \ ``Solution``\ . If the solution falls out of the grid bounds, the limits and content of the grid must be re-calculated.

   :param solution: \ ``Solution``\  considered to update the grid.
   :param solutionSet: \ ``SolutionSet``\  used to update the grid.

