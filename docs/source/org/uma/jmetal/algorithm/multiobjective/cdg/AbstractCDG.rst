.. java:import:: java.util ArrayList

.. java:import:: java.util Collections

.. java:import:: java.util Comparator

.. java:import:: java.util HashMap

.. java:import:: java.util List

.. java:import:: java.util Map

.. java:import:: java.util Random

.. java:import:: org.uma.jmetal.algorithm Algorithm

.. java:import:: org.uma.jmetal.operator CrossoverOperator

.. java:import:: org.uma.jmetal.operator MutationOperator

.. java:import:: org.uma.jmetal.problem Problem

.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util.pseudorandom JMetalRandom

.. java:import:: org.uma.jmetal.util.solutionattribute Ranking

.. java:import:: org.uma.jmetal.util.solutionattribute.impl DominanceRanking

AbstractCDG
===========

.. java:package:: org.uma.jmetal.algorithm.multiobjective.cdg
   :noindex:

.. java:type:: @SuppressWarnings public abstract class AbstractCDG<S extends Solution<?>> implements Algorithm<List<S>>

   Abstract class for implementing versions of the CDG algorithm.

   :author: Feng Zhang

Fields
------
badPopulation
^^^^^^^^^^^^^

.. java:field:: protected List<S> badPopulation
   :outertype: AbstractCDG

badSolution
^^^^^^^^^^^

.. java:field:: protected int[] badSolution
   :outertype: AbstractCDG

badSolutionNum
^^^^^^^^^^^^^^

.. java:field:: protected int badSolutionNum
   :outertype: AbstractCDG

border
^^^^^^

.. java:field:: protected List<List<S>> border
   :outertype: AbstractCDG

borderLength
^^^^^^^^^^^^

.. java:field:: protected int borderLength
   :outertype: AbstractCDG

childGridNum_
^^^^^^^^^^^^^

.. java:field:: protected int childGridNum_
   :outertype: AbstractCDG

childGrid_
^^^^^^^^^^

.. java:field:: protected int childGrid_
   :outertype: AbstractCDG

crossoverOperator
^^^^^^^^^^^^^^^^^

.. java:field:: protected CrossoverOperator<S> crossoverOperator
   :outertype: AbstractCDG

d_
^^

.. java:field:: protected double[] d_
   :outertype: AbstractCDG

evaluations
^^^^^^^^^^^

.. java:field:: protected int evaluations
   :outertype: AbstractCDG

gridDetalSum_
^^^^^^^^^^^^^

.. java:field:: protected double[][] gridDetalSum_
   :outertype: AbstractCDG

gridDetal_
^^^^^^^^^^

.. java:field:: protected int[] gridDetal_
   :outertype: AbstractCDG

idealPoint
^^^^^^^^^^

.. java:field:: protected double[] idealPoint
   :outertype: AbstractCDG

   Z vector in Zhang & Li paper

k_
^^

.. java:field:: protected int k_
   :outertype: AbstractCDG

maxEvaluations
^^^^^^^^^^^^^^

.. java:field:: protected int maxEvaluations
   :outertype: AbstractCDG

nadirPoint
^^^^^^^^^^

.. java:field:: protected double[] nadirPoint
   :outertype: AbstractCDG

neighborhood
^^^^^^^^^^^^

.. java:field:: protected int[][] neighborhood
   :outertype: AbstractCDG

neighborhoodNum
^^^^^^^^^^^^^^^

.. java:field:: protected int[] neighborhoodNum
   :outertype: AbstractCDG

neighborhoodSelectionProbability
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:field:: protected double neighborhoodSelectionProbability
   :outertype: AbstractCDG

   Delta in Zhang & Li paper

population
^^^^^^^^^^

.. java:field:: protected List<S> population
   :outertype: AbstractCDG

populationSize
^^^^^^^^^^^^^^

.. java:field:: protected int populationSize
   :outertype: AbstractCDG

problem
^^^^^^^

.. java:field:: protected Problem<S> problem
   :outertype: AbstractCDG

randomGenerator
^^^^^^^^^^^^^^^

.. java:field:: protected JMetalRandom randomGenerator
   :outertype: AbstractCDG

resultPopulationSize
^^^^^^^^^^^^^^^^^^^^

.. java:field:: protected int resultPopulationSize
   :outertype: AbstractCDG

sigma_
^^^^^^

.. java:field:: protected double sigma_
   :outertype: AbstractCDG

slimDetal_
^^^^^^^^^^

.. java:field:: protected int slimDetal_
   :outertype: AbstractCDG

spPopulationOrder
^^^^^^^^^^^^^^^^^

.. java:field:: protected List<Integer> spPopulationOrder
   :outertype: AbstractCDG

specialPopulation
^^^^^^^^^^^^^^^^^

.. java:field:: protected List<S> specialPopulation
   :outertype: AbstractCDG

subP
^^^^

.. java:field:: protected int[][] subP
   :outertype: AbstractCDG

subPNum
^^^^^^^

.. java:field:: protected int[] subPNum
   :outertype: AbstractCDG

subproblem
^^^^^^^^^^

.. java:field:: protected List<List<S>> subproblem
   :outertype: AbstractCDG

subproblemNum_
^^^^^^^^^^^^^^

.. java:field:: protected int subproblemNum_
   :outertype: AbstractCDG

t_
^^

.. java:field:: protected int t_
   :outertype: AbstractCDG

team
^^^^

.. java:field:: protected List<List<Integer>> team
   :outertype: AbstractCDG

tempBorder
^^^^^^^^^^

.. java:field:: protected List<List<S>> tempBorder
   :outertype: AbstractCDG

Constructors
------------
AbstractCDG
^^^^^^^^^^^

.. java:constructor:: public AbstractCDG(Problem<S> problem, int populationSize, int resultPopulationSize, int maxEvaluations, CrossoverOperator<S> crossoverOperator, double neighborhoodSelectionProbability, double sigma_, int k_, int t_, int subproblemNum_, int childGrid_, int childGridNum_)
   :outertype: AbstractCDG

Methods
-------
allocateSolution
^^^^^^^^^^^^^^^^

.. java:method:: protected void allocateSolution()
   :outertype: AbstractCDG

chooseNeighborType
^^^^^^^^^^^^^^^^^^

.. java:method:: protected NeighborType chooseNeighborType(int i)
   :outertype: AbstractCDG

chooseSolution
^^^^^^^^^^^^^^

.. java:method:: protected void chooseSolution()
   :outertype: AbstractCDG

chooseSpecialPopulation
^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: protected void chooseSpecialPopulation()
   :outertype: AbstractCDG

excludeBadSolution
^^^^^^^^^^^^^^^^^^

.. java:method:: protected void excludeBadSolution()
   :outertype: AbstractCDG

excludeBadSolution3
^^^^^^^^^^^^^^^^^^^

.. java:method:: protected void excludeBadSolution3()
   :outertype: AbstractCDG

getBorder
^^^^^^^^^

.. java:method:: protected void getBorder()
   :outertype: AbstractCDG

getG
^^^^

.. java:method:: protected int getG(S individual, int index)
   :outertype: AbstractCDG

getGridPos
^^^^^^^^^^

.. java:method:: protected int getGridPos(int j, double funValue)
   :outertype: AbstractCDG

getOrder
^^^^^^^^

.. java:method:: protected int getOrder(S individual)
   :outertype: AbstractCDG

getPos
^^^^^^

.. java:method:: protected int getPos(int i, int j, int k)
   :outertype: AbstractCDG

getRank
^^^^^^^

.. java:method:: protected int getRank(S individual, int index)
   :outertype: AbstractCDG

getResult
^^^^^^^^^

.. java:method:: @Override public List<S> getResult()
   :outertype: AbstractCDG

gridSystemSetup
^^^^^^^^^^^^^^^

.. java:method:: protected void gridSystemSetup()
   :outertype: AbstractCDG

gridSystemSetup3
^^^^^^^^^^^^^^^^

.. java:method:: protected void gridSystemSetup3()
   :outertype: AbstractCDG

group2
^^^^^^

.. java:method:: protected void group2()
   :outertype: AbstractCDG

group3
^^^^^^

.. java:method:: protected void group3()
   :outertype: AbstractCDG

individualObjRankSort
^^^^^^^^^^^^^^^^^^^^^

.. java:method:: protected void individualObjRankSort()
   :outertype: AbstractCDG

initialCDGAttributes
^^^^^^^^^^^^^^^^^^^^

.. java:method:: protected void initialCDGAttributes(S individual)
   :outertype: AbstractCDG

initialGridDetal
^^^^^^^^^^^^^^^^

.. java:method:: protected void initialGridDetal()
   :outertype: AbstractCDG

initializeIdealPoint
^^^^^^^^^^^^^^^^^^^^

.. java:method:: protected void initializeIdealPoint()
   :outertype: AbstractCDG

initializeNadirPoint
^^^^^^^^^^^^^^^^^^^^

.. java:method:: protected void initializeNadirPoint()
   :outertype: AbstractCDG

initializeNeighborhood
^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: protected void initializeNeighborhood()
   :outertype: AbstractCDG

   Initialize cdg neighborhoods

initializeNeighborhoodGrid
^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: protected void initializeNeighborhoodGrid()
   :outertype: AbstractCDG

initializeSubP2
^^^^^^^^^^^^^^^

.. java:method:: protected void initializeSubP2()
   :outertype: AbstractCDG

initializeSubP3
^^^^^^^^^^^^^^^

.. java:method:: protected void initializeSubP3()
   :outertype: AbstractCDG

isInner
^^^^^^^

.. java:method:: protected boolean isInner(S individual)
   :outertype: AbstractCDG

lexicographicSort
^^^^^^^^^^^^^^^^^

.. java:method:: protected void lexicographicSort()
   :outertype: AbstractCDG

matingSelection
^^^^^^^^^^^^^^^

.. java:method:: protected List<Integer> matingSelection(int subproblemId, int numberOfSolutionsToSelect, NeighborType neighbourType)
   :outertype: AbstractCDG

   :param subproblemId: the id of current subproblem
   :param neighbourType: neighbour type

parentSelection
^^^^^^^^^^^^^^^

.. java:method:: protected List<S> parentSelection(int subProblemId, NeighborType neighborType)
   :outertype: AbstractCDG

paretoDom
^^^^^^^^^

.. java:method:: protected boolean paretoDom(S individual, int i)
   :outertype: AbstractCDG

paretoFilter
^^^^^^^^^^^^

.. java:method:: protected void paretoFilter()
   :outertype: AbstractCDG

rankBasedSelection
^^^^^^^^^^^^^^^^^^

.. java:method:: protected void rankBasedSelection()
   :outertype: AbstractCDG

setG
^^^^

.. java:method:: protected void setG(S individual, int index, int value)
   :outertype: AbstractCDG

setIndividualObjRank
^^^^^^^^^^^^^^^^^^^^

.. java:method:: protected void setIndividualObjRank()
   :outertype: AbstractCDG

setOrder
^^^^^^^^

.. java:method:: protected void setOrder(S individual, int value)
   :outertype: AbstractCDG

setRank
^^^^^^^

.. java:method:: protected void setRank(S individual, int index, int value)
   :outertype: AbstractCDG

setSpIndividualRank
^^^^^^^^^^^^^^^^^^^

.. java:method:: protected void setSpIndividualRank()
   :outertype: AbstractCDG

subproblemSortl
^^^^^^^^^^^^^^^

.. java:method:: protected void subproblemSortl()
   :outertype: AbstractCDG

supplyBadSolution
^^^^^^^^^^^^^^^^^

.. java:method:: protected void supplyBadSolution()
   :outertype: AbstractCDG

updateBorder
^^^^^^^^^^^^

.. java:method:: protected void updateBorder()
   :outertype: AbstractCDG

updateIdealPoint
^^^^^^^^^^^^^^^^

.. java:method:: protected void updateIdealPoint(S individual)
   :outertype: AbstractCDG

updateNadirPoint
^^^^^^^^^^^^^^^^

.. java:method::  void updateNadirPoint()
   :outertype: AbstractCDG

updateNeighborhood
^^^^^^^^^^^^^^^^^^

.. java:method:: protected void updateNeighborhood()
   :outertype: AbstractCDG

