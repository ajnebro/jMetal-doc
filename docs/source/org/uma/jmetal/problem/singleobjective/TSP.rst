.. java:import:: org.uma.jmetal.problem.impl AbstractIntegerPermutationProblem

.. java:import:: org.uma.jmetal.solution PermutationSolution

.. java:import:: org.uma.jmetal.util JMetalException

TSP
===

.. java:package:: org.uma.jmetal.problem.singleobjective
   :noindex:

.. java:type:: @SuppressWarnings public class TSP extends AbstractIntegerPermutationProblem

   Class representing a single-objective TSP (Traveling Salesman Problem) problem. It accepts data files from TSPLIB: http://www.iwr.uni-heidelberg.de/groups/comopt/software/TSPLIB95/tsp/

Constructors
------------
TSP
^^^

.. java:constructor:: public TSP(String distanceFile) throws IOException
   :outertype: TSP

   Creates a new TSP problem instance

Methods
-------
evaluate
^^^^^^^^

.. java:method:: public void evaluate(PermutationSolution<Integer> solution)
   :outertype: TSP

   Evaluate() method

getPermutationLength
^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public int getPermutationLength()
   :outertype: TSP

