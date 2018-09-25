.. java:import:: org.uma.jmetal.algorithm Algorithm

.. java:import:: org.uma.jmetal.algorithm.multiobjective.moead.util MOEADUtils

.. java:import:: org.uma.jmetal.operator CrossoverOperator

.. java:import:: org.uma.jmetal.operator MutationOperator

.. java:import:: org.uma.jmetal.problem Problem

.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: org.uma.jmetal.util.point.impl IdealPoint

.. java:import:: org.uma.jmetal.util.point.impl NadirPoint

.. java:import:: org.uma.jmetal.util.pseudorandom JMetalRandom

.. java:import:: java.io BufferedReader

.. java:import:: java.io InputStream

.. java:import:: java.io InputStreamReader

.. java:import:: java.util ArrayList

.. java:import:: java.util List

.. java:import:: java.util StringTokenizer

AbstractMOEAD
=============

.. java:package:: org.uma.jmetal.algorithm.multiobjective.moead
   :noindex:

.. java:type:: @SuppressWarnings public abstract class AbstractMOEAD<S extends Solution<?>> implements Algorithm<List<S>>

   Abstract class for implementing versions of the MOEA/D algorithm.

   :author: Antonio J. Nebro

Fields
------
crossoverOperator
^^^^^^^^^^^^^^^^^

.. java:field:: protected CrossoverOperator<S> crossoverOperator
   :outertype: AbstractMOEAD

dataDirectory
^^^^^^^^^^^^^

.. java:field:: protected String dataDirectory
   :outertype: AbstractMOEAD

evaluations
^^^^^^^^^^^

.. java:field:: protected int evaluations
   :outertype: AbstractMOEAD

functionType
^^^^^^^^^^^^

.. java:field:: protected FunctionType functionType
   :outertype: AbstractMOEAD

idealPoint
^^^^^^^^^^

.. java:field:: protected IdealPoint idealPoint
   :outertype: AbstractMOEAD

   Z vector in Zhang & Li paper

indArray
^^^^^^^^

.. java:field:: protected Solution<?>[] indArray
   :outertype: AbstractMOEAD

jointPopulation
^^^^^^^^^^^^^^^

.. java:field:: protected List<S> jointPopulation
   :outertype: AbstractMOEAD

lambda
^^^^^^

.. java:field:: protected double[][] lambda
   :outertype: AbstractMOEAD

   Lambda vectors

maxEvaluations
^^^^^^^^^^^^^^

.. java:field:: protected int maxEvaluations
   :outertype: AbstractMOEAD

maximumNumberOfReplacedSolutions
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:field:: protected int maximumNumberOfReplacedSolutions
   :outertype: AbstractMOEAD

   nr in Zhang & Li paper

mutationOperator
^^^^^^^^^^^^^^^^

.. java:field:: protected MutationOperator<S> mutationOperator
   :outertype: AbstractMOEAD

nadirPoint
^^^^^^^^^^

.. java:field:: protected NadirPoint nadirPoint
   :outertype: AbstractMOEAD

neighborSize
^^^^^^^^^^^^

.. java:field:: protected int neighborSize
   :outertype: AbstractMOEAD

   T in Zhang & Li paper

neighborhood
^^^^^^^^^^^^

.. java:field:: protected int[][] neighborhood
   :outertype: AbstractMOEAD

neighborhoodSelectionProbability
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:field:: protected double neighborhoodSelectionProbability
   :outertype: AbstractMOEAD

   Delta in Zhang & Li paper

offspringPopulation
^^^^^^^^^^^^^^^^^^^

.. java:field:: protected List<S> offspringPopulation
   :outertype: AbstractMOEAD

population
^^^^^^^^^^

.. java:field:: protected List<S> population
   :outertype: AbstractMOEAD

populationSize
^^^^^^^^^^^^^^

.. java:field:: protected int populationSize
   :outertype: AbstractMOEAD

problem
^^^^^^^

.. java:field:: protected Problem<S> problem
   :outertype: AbstractMOEAD

randomGenerator
^^^^^^^^^^^^^^^

.. java:field:: protected JMetalRandom randomGenerator
   :outertype: AbstractMOEAD

resultPopulationSize
^^^^^^^^^^^^^^^^^^^^

.. java:field:: protected int resultPopulationSize
   :outertype: AbstractMOEAD

Constructors
------------
AbstractMOEAD
^^^^^^^^^^^^^

.. java:constructor:: public AbstractMOEAD(Problem<S> problem, int populationSize, int resultPopulationSize, int maxEvaluations, CrossoverOperator<S> crossoverOperator, MutationOperator<S> mutation, FunctionType functionType, String dataDirectory, double neighborhoodSelectionProbability, int maximumNumberOfReplacedSolutions, int neighborSize)
   :outertype: AbstractMOEAD

Methods
-------
chooseNeighborType
^^^^^^^^^^^^^^^^^^

.. java:method:: protected NeighborType chooseNeighborType()
   :outertype: AbstractMOEAD

fitnessFunction
^^^^^^^^^^^^^^^

.. java:method::  double fitnessFunction(S individual, double[] lambda) throws JMetalException
   :outertype: AbstractMOEAD

getResult
^^^^^^^^^

.. java:method:: @Override public List<S> getResult()
   :outertype: AbstractMOEAD

initializeNeighborhood
^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: protected void initializeNeighborhood()
   :outertype: AbstractMOEAD

   Initialize neighborhoods

initializeUniformWeight
^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: protected void initializeUniformWeight()
   :outertype: AbstractMOEAD

   Initialize weight vectors

matingSelection
^^^^^^^^^^^^^^^

.. java:method:: protected List<Integer> matingSelection(int subproblemId, int numberOfSolutionsToSelect, NeighborType neighbourType)
   :outertype: AbstractMOEAD

   :param subproblemId: the id of current subproblem
   :param neighbourType: neighbour type

parentSelection
^^^^^^^^^^^^^^^

.. java:method:: protected List<S> parentSelection(int subProblemId, NeighborType neighborType)
   :outertype: AbstractMOEAD

updateNeighborhood
^^^^^^^^^^^^^^^^^^

.. java:method:: @SuppressWarnings protected void updateNeighborhood(S individual, int subProblemId, NeighborType neighborType) throws JMetalException
   :outertype: AbstractMOEAD

   Update neighborhood method

   :param individual:
   :param subProblemId:
   :param neighborType:
   :throws JMetalException:

