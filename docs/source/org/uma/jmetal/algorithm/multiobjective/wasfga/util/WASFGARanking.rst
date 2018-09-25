.. java:import:: org.uma.jmetal.algorithm.multiobjective.mombi.util AbstractUtilityFunctionsSet

.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util.solutionattribute Ranking

.. java:import:: org.uma.jmetal.util.solutionattribute.impl GenericSolutionAttribute

.. java:import:: org.uma.jmetal.util.solutionattribute.impl NumberOfViolatedConstraints

.. java:import:: org.uma.jmetal.util.solutionattribute.impl OverallConstraintViolation

.. java:import:: java.util ArrayList

.. java:import:: java.util Arrays

.. java:import:: java.util LinkedList

.. java:import:: java.util List

WASFGARanking
=============

.. java:package:: org.uma.jmetal.algorithm.multiobjective.wasfga.util
   :noindex:

.. java:type:: public class WASFGARanking<S extends Solution<?>> extends GenericSolutionAttribute<S, Integer> implements Ranking<S>

   :author: Rubén Saborido Implementation of the ranking procedure for the preference based algorithm named WASF-GA on jMetal5.0 It classifies solutions into different fronts. If the problem contains constraints, after feasible solutions it classifies the unfeasible solutions into fronts: - Each unfeasible solutions goes into a different front. - Unfeasible solutions with lower number of violated constraints are preferred. - If two solutions have equal number of violated constraints it compares the overall constraint values. - If two solutions have equal overall constraint values it compares de values of the utility function.

Constructors
------------
WASFGARanking
^^^^^^^^^^^^^

.. java:constructor:: public WASFGARanking(AbstractUtilityFunctionsSet<S> utilityFunctions)
   :outertype: WASFGARanking

Methods
-------
computeRanking
^^^^^^^^^^^^^^

.. java:method:: @Override public Ranking<S> computeRanking(List<S> population)
   :outertype: WASFGARanking

getNumberOfSubfronts
^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public int getNumberOfSubfronts()
   :outertype: WASFGARanking

getSubfront
^^^^^^^^^^^

.. java:method:: @Override public List<S> getSubfront(int rank)
   :outertype: WASFGARanking

getUtilityFunctions
^^^^^^^^^^^^^^^^^^^

.. java:method:: public AbstractUtilityFunctionsSet<S> getUtilityFunctions()
   :outertype: WASFGARanking

rankUnfeasibleSolutions
^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: protected int[] rankUnfeasibleSolutions(List<S> population)
   :outertype: WASFGARanking

   Obtain the rank of each solution in a list of unfeasible solutions

   :param population: List of unfeasible solutions
   :return: The rank of each unfeasible solutions

