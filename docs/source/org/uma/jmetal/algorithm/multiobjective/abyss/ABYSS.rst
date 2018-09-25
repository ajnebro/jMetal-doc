.. java:import:: org.uma.jmetal.algorithm.impl AbstractScatterSearch

.. java:import:: org.uma.jmetal.algorithm.multiobjective.abyss.util MarkAttribute

.. java:import:: org.uma.jmetal.operator CrossoverOperator

.. java:import:: org.uma.jmetal.operator LocalSearchOperator

.. java:import:: org.uma.jmetal.problem ConstrainedProblem

.. java:import:: org.uma.jmetal.problem DoubleProblem

.. java:import:: org.uma.jmetal.problem Problem

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.util SolutionUtils

.. java:import:: org.uma.jmetal.util.archive Archive

.. java:import:: org.uma.jmetal.util.archive.impl CrowdingDistanceArchive

.. java:import:: org.uma.jmetal.util.comparator CrowdingDistanceComparator

.. java:import:: org.uma.jmetal.util.comparator DominanceComparator

.. java:import:: org.uma.jmetal.util.comparator EqualSolutionsComparator

.. java:import:: org.uma.jmetal.util.comparator StrengthFitnessComparator

.. java:import:: org.uma.jmetal.util.pseudorandom JMetalRandom

.. java:import:: org.uma.jmetal.util.solutionattribute.impl DistanceToSolutionListAttribute

.. java:import:: org.uma.jmetal.util.solutionattribute.impl StrengthRawFitness

.. java:import:: javax.management JMException

.. java:import:: java.util ArrayList

.. java:import:: java.util Collections

.. java:import:: java.util Comparator

.. java:import:: java.util List

ABYSS
=====

.. java:package:: org.uma.jmetal.algorithm.multiobjective.abyss
   :noindex:

.. java:type:: @SuppressWarnings public class ABYSS extends AbstractScatterSearch<DoubleSolution, List<DoubleSolution>>

   This class implements the AbYSS algorithm, a multiobjective scatter search metaheuristics, which is described in: A.J. Nebro, F. Luna, E. Alba, B. Dorronsoro, J.J. Durillo, A. Beham "AbYSS: Adapting Scatter Search to Multiobjective Optimization." IEEE Transactions on Evolutionary Computation. Vol. 12, No. 4 (August 2008), pp. 439-457

   :author: Antonio J. Nebro , Cristobal Barba

Fields
------
archive
^^^^^^^

.. java:field:: protected Archive<DoubleSolution> archive
   :outertype: ABYSS

archiveSize
^^^^^^^^^^^

.. java:field:: protected final int archiveSize
   :outertype: ABYSS

crossover
^^^^^^^^^

.. java:field:: protected CrossoverOperator<DoubleSolution> crossover
   :outertype: ABYSS

crowdingDistanceComparator
^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:field:: protected Comparator<DoubleSolution> crowdingDistanceComparator
   :outertype: ABYSS

distanceToSolutionListAttribute
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:field:: protected DistanceToSolutionListAttribute distanceToSolutionListAttribute
   :outertype: ABYSS

dominanceComparator
^^^^^^^^^^^^^^^^^^^

.. java:field:: protected Comparator<DoubleSolution> dominanceComparator
   :outertype: ABYSS

equalComparator
^^^^^^^^^^^^^^^

.. java:field:: protected Comparator<DoubleSolution> equalComparator
   :outertype: ABYSS

evaluations
^^^^^^^^^^^

.. java:field:: protected int evaluations
   :outertype: ABYSS

fitnessComparator
^^^^^^^^^^^^^^^^^

.. java:field:: protected Comparator<DoubleSolution> fitnessComparator
   :outertype: ABYSS

frequency
^^^^^^^^^

.. java:field:: protected int[][] frequency
   :outertype: ABYSS

localSearch
^^^^^^^^^^^

.. java:field:: protected LocalSearchOperator<DoubleSolution> localSearch
   :outertype: ABYSS

marked
^^^^^^

.. java:field:: protected MarkAttribute marked
   :outertype: ABYSS

maxEvaluations
^^^^^^^^^^^^^^

.. java:field:: protected final int maxEvaluations
   :outertype: ABYSS

numberOfSubRanges
^^^^^^^^^^^^^^^^^

.. java:field:: protected int numberOfSubRanges
   :outertype: ABYSS

   These variables are used in the diversification method.

problem
^^^^^^^

.. java:field:: protected final Problem<DoubleSolution> problem
   :outertype: ABYSS

randomGenerator
^^^^^^^^^^^^^^^

.. java:field:: protected JMetalRandom randomGenerator
   :outertype: ABYSS

referenceSet1
^^^^^^^^^^^^^

.. java:field:: protected List<DoubleSolution> referenceSet1
   :outertype: ABYSS

referenceSet1Size
^^^^^^^^^^^^^^^^^

.. java:field:: protected final int referenceSet1Size
   :outertype: ABYSS

referenceSet2
^^^^^^^^^^^^^

.. java:field:: protected List<DoubleSolution> referenceSet2
   :outertype: ABYSS

referenceSet2Size
^^^^^^^^^^^^^^^^^

.. java:field:: protected final int referenceSet2Size
   :outertype: ABYSS

reverseFrequency
^^^^^^^^^^^^^^^^

.. java:field:: protected int[][] reverseFrequency
   :outertype: ABYSS

strengthRawFitness
^^^^^^^^^^^^^^^^^^

.. java:field:: protected StrengthRawFitness<DoubleSolution> strengthRawFitness
   :outertype: ABYSS

sumOfFrequencyValues
^^^^^^^^^^^^^^^^^^^^

.. java:field:: protected int[] sumOfFrequencyValues
   :outertype: ABYSS

sumOfReverseFrequencyValues
^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:field:: protected int[] sumOfReverseFrequencyValues
   :outertype: ABYSS

Constructors
------------
ABYSS
^^^^^

.. java:constructor:: public ABYSS(DoubleProblem problem, int maxEvaluations, int populationSize, int referenceSet1Size, int referenceSet2Size, int archiveSize, Archive<DoubleSolution> archive, LocalSearchOperator<DoubleSolution> localSearch, CrossoverOperator<DoubleSolution> crossoverOperator, int numberOfSubRanges)
   :outertype: ABYSS

Methods
-------
buildNewReferenceSet1
^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public void buildNewReferenceSet1()
   :outertype: ABYSS

   Build the referenceSet1 by moving the best referenceSet1Size individuals, according to a fitness comparator, from the population to the referenceSet1

buildNewReferenceSet2
^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public void buildNewReferenceSet2()
   :outertype: ABYSS

   Build the referenceSet2 by moving to it the most diverse referenceSet2Size individuals from the population in respect to the referenceSet1. The size of the referenceSet2 can be lower than referenceSet2Size depending on the current size of the population

diversificationGeneration
^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public DoubleSolution diversificationGeneration()
   :outertype: ABYSS

generatePairsFromSolutionList
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public List<List<DoubleSolution>> generatePairsFromSolutionList(List<DoubleSolution> solutionList)
   :outertype: ABYSS

   Generate all pair combinations of the referenceSet1

getDescription
^^^^^^^^^^^^^^

.. java:method:: @Override public String getDescription()
   :outertype: ABYSS

getName
^^^^^^^

.. java:method:: @Override public String getName()
   :outertype: ABYSS

getResult
^^^^^^^^^

.. java:method:: @Override public List<DoubleSolution> getResult()
   :outertype: ABYSS

improvement
^^^^^^^^^^^

.. java:method:: @Override public DoubleSolution improvement(DoubleSolution solution)
   :outertype: ABYSS

isStoppingConditionReached
^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public boolean isStoppingConditionReached()
   :outertype: ABYSS

refSet1Test
^^^^^^^^^^^

.. java:method:: public boolean refSet1Test(DoubleSolution solution)
   :outertype: ABYSS

   Tries to update the reference set one with a solution

   :param solution: The \ ``Solution``\
   :return: true if the \ ``Solution``\  has been inserted, false otherwise.

refSet2Test
^^^^^^^^^^^

.. java:method:: public boolean refSet2Test(DoubleSolution solution)
   :outertype: ABYSS

   Try to update the reference set 2 with a \ ``Solution``\

   :param solution: The \ ``Solution``\
   :throws JMException:
   :return: true if the \ ``Solution``\  has been inserted, false otherwise.

referenceSetUpdate
^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public void referenceSetUpdate()
   :outertype: ABYSS

   Build the reference set after the initialization phase

referenceSetUpdate
^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public void referenceSetUpdate(DoubleSolution solution)
   :outertype: ABYSS

   Update the reference set with a new solution

   :param solution:

restart
^^^^^^^

.. java:method:: @Override public void restart()
   :outertype: ABYSS

restartConditionIsFulfilled
^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public boolean restartConditionIsFulfilled(List<DoubleSolution> combinedSolutions)
   :outertype: ABYSS

solutionCombination
^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public List<DoubleSolution> solutionCombination(List<List<DoubleSolution>> solutionList)
   :outertype: ABYSS

subsetGeneration
^^^^^^^^^^^^^^^^

.. java:method:: @Override public List<List<DoubleSolution>> subsetGeneration()
   :outertype: ABYSS

   Subset generation method

