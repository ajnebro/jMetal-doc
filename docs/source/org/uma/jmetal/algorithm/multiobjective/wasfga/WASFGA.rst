.. java:import:: org.uma.jmetal.algorithm InteractiveAlgorithm

.. java:import:: org.uma.jmetal.algorithm.multiobjective.mombi AbstractMOMBI

.. java:import:: org.uma.jmetal.algorithm.multiobjective.mombi.util ASFWASFGA

.. java:import:: org.uma.jmetal.algorithm.multiobjective.mombi.util AbstractUtilityFunctionsSet

.. java:import:: org.uma.jmetal.algorithm.multiobjective.wasfga.util WASFGARanking

.. java:import:: org.uma.jmetal.algorithm.multiobjective.wasfga.util WeightVectors

.. java:import:: org.uma.jmetal.operator CrossoverOperator

.. java:import:: org.uma.jmetal.operator MutationOperator

.. java:import:: org.uma.jmetal.operator SelectionOperator

.. java:import:: org.uma.jmetal.problem Problem

.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: org.uma.jmetal.util SolutionListUtils

.. java:import:: org.uma.jmetal.util.evaluator SolutionListEvaluator

.. java:import:: org.uma.jmetal.util.solutionattribute Ranking

.. java:import:: java.util ArrayList

.. java:import:: java.util List

WASFGA
======

.. java:package:: org.uma.jmetal.algorithm.multiobjective.wasfga
   :noindex:

.. java:type:: public class WASFGA<S extends Solution<?>> extends AbstractMOMBI<S> implements InteractiveAlgorithm<S, List<S>>

   Implementation of the preference based algorithm named WASF-GA on jMetal5.0

   :author: Juanjo Durillo This algorithm is described in the paper: A.B. Ruiz, R. Saborido, M. Luque "A Preference-based Evolutionary Algorithm for Multiobjective Optimization: The Weighting Achievement Scalarizing Function Genetic Algorithm". Journal of Global Optimization. May 2015, Volume 62, Issue 1, pp 101-129 DOI = {10.1007/s10898-014-0214-y}

Fields
------
epsilon
^^^^^^^

.. java:field:: protected double epsilon
   :outertype: WASFGA

evaluations
^^^^^^^^^^^

.. java:field:: protected int evaluations
   :outertype: WASFGA

maxEvaluations
^^^^^^^^^^^^^^

.. java:field:: protected int maxEvaluations
   :outertype: WASFGA

weights
^^^^^^^

.. java:field:: protected double[][] weights
   :outertype: WASFGA

Constructors
------------
WASFGA
^^^^^^

.. java:constructor:: public WASFGA(Problem<S> problem, int populationSize, int maxIterations, CrossoverOperator<S> crossoverOperator, MutationOperator<S> mutationOperator, SelectionOperator<List<S>, S> selectionOperator, SolutionListEvaluator<S> evaluator, double epsilon, List<Double> referencePoint, String weightVectorsFileName)
   :outertype: WASFGA

   Constructor

   :param problem: Problem to solve

WASFGA
^^^^^^

.. java:constructor:: public WASFGA(Problem<S> problem, int populationSize, int maxIterations, CrossoverOperator<S> crossoverOperator, MutationOperator<S> mutationOperator, SelectionOperator<List<S>, S> selectionOperator, SolutionListEvaluator<S> evaluator, double epsilon, List<Double> referencePoint)
   :outertype: WASFGA

   Constructor

   :param problem: Problem to solve

Methods
-------
addLastRankedSolutionsToPopulation
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: protected void addLastRankedSolutionsToPopulation(Ranking<S> ranking, int index, List<S> population)
   :outertype: WASFGA

addRankedSolutionsToPopulation
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: protected void addRankedSolutionsToPopulation(Ranking<S> ranking, int index, List<S> population)
   :outertype: WASFGA

computeRanking
^^^^^^^^^^^^^^

.. java:method:: protected Ranking<S> computeRanking(List<S> solutionList)
   :outertype: WASFGA

createUtilityFunction
^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public AbstractUtilityFunctionsSet<S> createUtilityFunction()
   :outertype: WASFGA

getDescription
^^^^^^^^^^^^^^

.. java:method:: @Override public String getDescription()
   :outertype: WASFGA

getName
^^^^^^^

.. java:method:: @Override public String getName()
   :outertype: WASFGA

getNonDominatedSolutions
^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: protected List<S> getNonDominatedSolutions(List<S> solutionList)
   :outertype: WASFGA

getPopulationSize
^^^^^^^^^^^^^^^^^

.. java:method:: public int getPopulationSize()
   :outertype: WASFGA

getResult
^^^^^^^^^

.. java:method:: @Override public List<S> getResult()
   :outertype: WASFGA

replacement
^^^^^^^^^^^

.. java:method:: @Override protected List<S> replacement(List<S> population, List<S> offspringPopulation)
   :outertype: WASFGA

selectBest
^^^^^^^^^^

.. java:method:: protected List<S> selectBest(Ranking<S> ranking)
   :outertype: WASFGA

specificMOEAComputations
^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public void specificMOEAComputations()
   :outertype: WASFGA

updatePointOfInterest
^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public void updatePointOfInterest(List<Double> newPointOfInterest)
   :outertype: WASFGA

