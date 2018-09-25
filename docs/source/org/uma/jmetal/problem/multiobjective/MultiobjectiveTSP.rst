.. java:import:: org.uma.jmetal.problem.impl AbstractIntegerPermutationProblem

.. java:import:: org.uma.jmetal.solution PermutationSolution

.. java:import:: org.uma.jmetal.util JMetalException

MultiobjectiveTSP
=================

.. java:package:: org.uma.jmetal.problem.multiobjective
   :noindex:

.. java:type:: @SuppressWarnings public class MultiobjectiveTSP extends AbstractIntegerPermutationProblem

   Class representing a bi-objective TSP (Traveling Salesman Problem) problem. It accepts data files from TSPLIB: http://www.iwr.uni-heidelberg.de/groups/comopt/software/TSPLIB95/tsp/

Fields
------
costMatrix
^^^^^^^^^^

.. java:field:: protected double[][] costMatrix
   :outertype: MultiobjectiveTSP

distanceMatrix
^^^^^^^^^^^^^^

.. java:field:: protected double[][] distanceMatrix
   :outertype: MultiobjectiveTSP

numberOfCities
^^^^^^^^^^^^^^

.. java:field:: protected int numberOfCities
   :outertype: MultiobjectiveTSP

Constructors
------------
MultiobjectiveTSP
^^^^^^^^^^^^^^^^^

.. java:constructor:: public MultiobjectiveTSP(String distanceFile, String costFile) throws IOException
   :outertype: MultiobjectiveTSP

   Creates a new MultiobjectiveTSP problem instance

Methods
-------
evaluate
^^^^^^^^

.. java:method:: public void evaluate(PermutationSolution<Integer> solution)
   :outertype: MultiobjectiveTSP

   Evaluate() method

getPermutationLength
^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public int getPermutationLength()
   :outertype: MultiobjectiveTSP

