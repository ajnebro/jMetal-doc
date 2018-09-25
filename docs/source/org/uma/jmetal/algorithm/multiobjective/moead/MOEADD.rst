.. java:import:: org.uma.jmetal.algorithm.multiobjective.moead.util MOEADUtils

.. java:import:: org.uma.jmetal.operator CrossoverOperator

.. java:import:: org.uma.jmetal.operator MutationOperator

.. java:import:: org.uma.jmetal.problem Problem

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.util.point.impl IdealPoint

.. java:import:: org.uma.jmetal.util.point.impl NadirPoint

.. java:import:: org.uma.jmetal.util.solutionattribute Ranking

.. java:import:: org.uma.jmetal.util.solutionattribute.impl DominanceRanking

.. java:import:: java.util ArrayList

.. java:import:: java.util List

MOEADD
======

.. java:package:: org.uma.jmetal.algorithm.multiobjective.moead
   :noindex:

.. java:type:: public class MOEADD<S extends DoubleSolution> extends AbstractMOEAD<S>

Fields
------
numRanks
^^^^^^^^

.. java:field:: protected int numRanks
   :outertype: MOEADD

rankIdx
^^^^^^^

.. java:field:: protected int[][] rankIdx
   :outertype: MOEADD

ranking
^^^^^^^

.. java:field:: protected Ranking ranking
   :outertype: MOEADD

subregionDist
^^^^^^^^^^^^^

.. java:field:: protected double[][] subregionDist
   :outertype: MOEADD

subregionIdx
^^^^^^^^^^^^

.. java:field:: protected int[][] subregionIdx
   :outertype: MOEADD

Constructors
------------
MOEADD
^^^^^^

.. java:constructor:: public MOEADD(Problem<S> problem, int populationSize, int resultPopulationSize, int maxEvaluations, CrossoverOperator<S> crossoverOperator, MutationOperator<S> mutation, AbstractMOEAD.FunctionType functionType, String dataDirectory, double neighborhoodSelectionProbability, int maximumNumberOfReplacedSolutions, int neighborSize)
   :outertype: MOEADD

Methods
-------
calculateDistance
^^^^^^^^^^^^^^^^^

.. java:method:: public double calculateDistance(S individual, double[] lambda, double[] z_, double[] nz_)
   :outertype: MOEADD

   Calculate the perpendicular distance between the solution and reference line

calculateDistance2
^^^^^^^^^^^^^^^^^^

.. java:method:: public double calculateDistance2(S indiv, double[] lambda, double[] z_, double[] nz_)
   :outertype: MOEADD

checkDominance
^^^^^^^^^^^^^^

.. java:method:: public int checkDominance(S a, S b)
   :outertype: MOEADD

   check the dominance relationship between a and b: 1 -> a dominates b, -1 -> b dominates a 0 -> non-dominated with each other

computeRanking
^^^^^^^^^^^^^^

.. java:method:: protected Ranking<S> computeRanking(List<S> solutionList)
   :outertype: MOEADD

countOnes
^^^^^^^^^

.. java:method:: public int countOnes(int location)
   :outertype: MOEADD

   Count the number of 1s in the 'location'th subregion

countRankOnes
^^^^^^^^^^^^^

.. java:method:: public int countRankOnes(int location)
   :outertype: MOEADD

   count the number of 1s in a row of rank matrix

countTest
^^^^^^^^^

.. java:method:: public int countTest()
   :outertype: MOEADD

deleteCrowdIndiv_diff
^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public void deleteCrowdIndiv_diff(int crowdIdx, int curLocation, int nicheCount, S indiv)
   :outertype: MOEADD

   delete one solution from the most crowded subregion, which is different from indiv's subregion. just use indiv to replace the worst solution in that subregion

deleteCrowdIndiv_same
^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public void deleteCrowdIndiv_same(int crowdIdx, int nicheCount, double indivFitness, S indiv)
   :outertype: MOEADD

   delete one solution from the most crowded subregion, which is indiv's subregion. Compare indiv's fitness value and the worst one in this subregion

deleteCrowdRegion1
^^^^^^^^^^^^^^^^^^

.. java:method:: public void deleteCrowdRegion1(S indiv, int location)
   :outertype: MOEADD

   Delete a solution from the most crowded subregion (this function only happens when: it should delete 'indiv' based on traditional method. However, the subregion of 'indiv' only has one solution, so it should be kept)

deleteCrowdRegion2
^^^^^^^^^^^^^^^^^^

.. java:method:: public void deleteCrowdRegion2(S indiv, int location)
   :outertype: MOEADD

   delete a solution from the most crowded subregion (this function happens when: it should delete the solution in the 'parentLocation' subregion, but since this subregion only has one solution, it should be kept)

deleteRankOne
^^^^^^^^^^^^^

.. java:method:: public void deleteRankOne(S indiv, int location)
   :outertype: MOEADD

   if there is only one non-domination level (i.e., all solutions are non-dominated with each other), we should delete a solution from the most crowded subregion

findPosition
^^^^^^^^^^^^

.. java:method:: public int findPosition(S indiv)
   :outertype: MOEADD

   find the index of the solution 'indiv' in the population

findRegion
^^^^^^^^^^

.. java:method:: public int findRegion(int idx)
   :outertype: MOEADD

   find the subregion of the 'idx'th solution in the population

getDescription
^^^^^^^^^^^^^^

.. java:method:: @Override public String getDescription()
   :outertype: MOEADD

getName
^^^^^^^

.. java:method:: @Override public String getName()
   :outertype: MOEADD

initPopulation
^^^^^^^^^^^^^^

.. java:method:: public void initPopulation()
   :outertype: MOEADD

   Initialize the population

innerproduct
^^^^^^^^^^^^

.. java:method:: public double innerproduct(double[] vec1, double[] vec2)
   :outertype: MOEADD

   Calculate the dot product of two vectors

matingSelection
^^^^^^^^^^^^^^^

.. java:method:: public List<S> matingSelection(int cid, int type)
   :outertype: MOEADD

   Select two parents for reproduction

nondominated_sorting_add
^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public int nondominated_sorting_add(S indiv)
   :outertype: MOEADD

   update the non-domination level when adding a solution

nondominated_sorting_delete
^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public void nondominated_sorting_delete(S indiv)
   :outertype: MOEADD

   update the non-domination level structure after deleting a solution

norm_vector
^^^^^^^^^^^

.. java:method:: public double norm_vector(double[] z)
   :outertype: MOEADD

   Calculate the norm of the vector

replace
^^^^^^^

.. java:method:: public void replace(int position, S solution)
   :outertype: MOEADD

run
^^^

.. java:method:: @Override public void run()
   :outertype: MOEADD

setLocation
^^^^^^^^^^^

.. java:method:: public void setLocation(S indiv, double[] z_, double[] nz_)
   :outertype: MOEADD

   Set the location of a solution based on the orthogonal distance

sumFitness
^^^^^^^^^^

.. java:method:: public double sumFitness(int location)
   :outertype: MOEADD

   calculate the sum of fitnesses of solutions in the location subregion

updateArchive
^^^^^^^^^^^^^

.. java:method:: public void updateArchive(S indiv)
   :outertype: MOEADD

   update the parent population by using the ENLU method, instead of fast non-dominated sorting

