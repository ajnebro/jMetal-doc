.. java:import:: org.uma.jmetal.algorithm.multiobjective.moead.util MOEADUtils

.. java:import:: org.uma.jmetal.operator CrossoverOperator

.. java:import:: org.uma.jmetal.operator MutationOperator

.. java:import:: org.uma.jmetal.operator.impl.crossover DifferentialEvolutionCrossover

.. java:import:: org.uma.jmetal.problem Problem

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: org.uma.jmetal.util.pseudorandom JMetalRandom

.. java:import:: java.util ArrayList

.. java:import:: java.util LinkedList

.. java:import:: java.util List

MOEADSTM
========

.. java:package:: org.uma.jmetal.algorithm.multiobjective.moead
   :noindex:

.. java:type:: @SuppressWarnings public class MOEADSTM extends AbstractMOEAD<DoubleSolution>

   Class implementing the MOEA/D-STM algorithm described in : K. Li, Q. Zhang, S. Kwong, M. Li and R. Wang, "Stable Matching-Based Selection in Evolutionary Multiobjective Optimization", IEEE Transactions on Evolutionary Computation, 18(6): 909-923, 2014. DOI: 10.1109/TEVC.2013.2293776

   :author: Ke Li

Fields
------
differentialEvolutionCrossover
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:field:: protected DifferentialEvolutionCrossover differentialEvolutionCrossover
   :outertype: MOEADSTM

frequency
^^^^^^^^^

.. java:field:: protected int[] frequency
   :outertype: MOEADSTM

randomGenerator
^^^^^^^^^^^^^^^

.. java:field::  JMetalRandom randomGenerator
   :outertype: MOEADSTM

savedValues
^^^^^^^^^^^

.. java:field:: protected DoubleSolution[] savedValues
   :outertype: MOEADSTM

utility
^^^^^^^

.. java:field:: protected double[] utility
   :outertype: MOEADSTM

Constructors
------------
MOEADSTM
^^^^^^^^

.. java:constructor:: public MOEADSTM(Problem<DoubleSolution> problem, int populationSize, int resultPopulationSize, int maxEvaluations, MutationOperator<DoubleSolution> mutation, CrossoverOperator<DoubleSolution> crossover, FunctionType functionType, String dataDirectory, double neighborhoodSelectionProbability, int maximumNumberOfReplacedSolutions, int neighborSize)
   :outertype: MOEADSTM

Methods
-------
calculateDistance
^^^^^^^^^^^^^^^^^

.. java:method:: public double calculateDistance(DoubleSolution individual, double[] lambda)
   :outertype: MOEADSTM

   Calculate the perpendicular distance between the solution and reference line

calculateDistance2
^^^^^^^^^^^^^^^^^^

.. java:method:: public double calculateDistance2(DoubleSolution individual, double[] lambda)
   :outertype: MOEADSTM

   Calculate the perpendicular distance between the solution and reference line

getDescription
^^^^^^^^^^^^^^

.. java:method:: @Override public String getDescription()
   :outertype: MOEADSTM

getName
^^^^^^^

.. java:method:: @Override public String getName()
   :outertype: MOEADSTM

getResult
^^^^^^^^^

.. java:method:: @Override public List<DoubleSolution> getResult()
   :outertype: MOEADSTM

initializePopulation
^^^^^^^^^^^^^^^^^^^^

.. java:method:: protected void initializePopulation()
   :outertype: MOEADSTM

innerproduct
^^^^^^^^^^^^

.. java:method:: public double innerproduct(double[] vec1, double[] vec2)
   :outertype: MOEADSTM

   Calculate the dot product of two vectors

norm_vector
^^^^^^^^^^^

.. java:method:: public double norm_vector(double[] z)
   :outertype: MOEADSTM

   Calculate the norm of the vector

prefers
^^^^^^^

.. java:method:: public boolean prefers(int x, int y, int[] womanPref, int size)
   :outertype: MOEADSTM

   Returns true in case that a given woman prefers x to y.

run
^^^

.. java:method:: @Override public void run()
   :outertype: MOEADSTM

stableMatching
^^^^^^^^^^^^^^

.. java:method:: public int[] stableMatching(int[][] manPref, int[][] womanPref, int menSize, int womenSize)
   :outertype: MOEADSTM

   Return the stable matching between 'subproblems' and 'solutions' ('subproblems' propose first). It is worth noting that the number of solutions is larger than that of the subproblems.

stmSelection
^^^^^^^^^^^^

.. java:method:: public void stmSelection()
   :outertype: MOEADSTM

   Select the next parent population, based on the stable matching criteria

tourSelection
^^^^^^^^^^^^^

.. java:method:: public List<Integer> tourSelection(int depth)
   :outertype: MOEADSTM

utilityFunction
^^^^^^^^^^^^^^^

.. java:method:: public void utilityFunction() throws JMetalException
   :outertype: MOEADSTM

