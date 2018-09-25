.. java:import:: org.uma.jmetal.algorithm.multiobjective.moead MOEADBuilder

.. java:import:: org.uma.jmetal.operator CrossoverOperator

.. java:import:: org.uma.jmetal.operator MutationOperator

.. java:import:: org.uma.jmetal.operator.impl.crossover DifferentialEvolutionCrossover

.. java:import:: org.uma.jmetal.operator.impl.mutation PolynomialMutation

.. java:import:: org.uma.jmetal.problem Problem

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.util AlgorithmBuilder

CDGBuilder
==========

.. java:package:: org.uma.jmetal.algorithm.multiobjective.cdg
   :noindex:

.. java:type:: public class CDGBuilder implements AlgorithmBuilder<AbstractCDG<DoubleSolution>>

   Builder class for algorithm CDG

   :author: Feng Zhang

Fields
------
childGridNum_
^^^^^^^^^^^^^

.. java:field:: protected int childGridNum_
   :outertype: CDGBuilder

childGrid_
^^^^^^^^^^

.. java:field:: protected int childGrid_
   :outertype: CDGBuilder

crossover
^^^^^^^^^

.. java:field:: protected CrossoverOperator<DoubleSolution> crossover
   :outertype: CDGBuilder

k_
^^

.. java:field:: protected int k_
   :outertype: CDGBuilder

maxEvaluations
^^^^^^^^^^^^^^

.. java:field:: protected int maxEvaluations
   :outertype: CDGBuilder

neighborhoodSelectionProbability
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:field:: protected double neighborhoodSelectionProbability
   :outertype: CDGBuilder

   Delta in Zhang & Li paper

numberOfThreads
^^^^^^^^^^^^^^^

.. java:field:: protected int numberOfThreads
   :outertype: CDGBuilder

populationSize
^^^^^^^^^^^^^^

.. java:field:: protected int populationSize
   :outertype: CDGBuilder

problem
^^^^^^^

.. java:field:: protected Problem<DoubleSolution> problem
   :outertype: CDGBuilder

resultPopulationSize
^^^^^^^^^^^^^^^^^^^^

.. java:field:: protected int resultPopulationSize
   :outertype: CDGBuilder

sigma_
^^^^^^

.. java:field:: protected double sigma_
   :outertype: CDGBuilder

subproblemNum_
^^^^^^^^^^^^^^

.. java:field:: protected int subproblemNum_
   :outertype: CDGBuilder

t_
^^

.. java:field:: protected int t_
   :outertype: CDGBuilder

Constructors
------------
CDGBuilder
^^^^^^^^^^

.. java:constructor:: public CDGBuilder(Problem<DoubleSolution> problem)
   :outertype: CDGBuilder

   Constructor

Methods
-------
build
^^^^^

.. java:method:: public AbstractCDG<DoubleSolution> build()
   :outertype: CDGBuilder

getChildGrid
^^^^^^^^^^^^

.. java:method:: public int getChildGrid()
   :outertype: CDGBuilder

getChildGridNum
^^^^^^^^^^^^^^^

.. java:method:: public int getChildGridNum()
   :outertype: CDGBuilder

getCrossover
^^^^^^^^^^^^

.. java:method:: public CrossoverOperator<DoubleSolution> getCrossover()
   :outertype: CDGBuilder

getK
^^^^

.. java:method:: public int getK()
   :outertype: CDGBuilder

getMaxEvaluations
^^^^^^^^^^^^^^^^^

.. java:method:: public int getMaxEvaluations()
   :outertype: CDGBuilder

getNeighborhoodSelectionProbability
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public double getNeighborhoodSelectionProbability()
   :outertype: CDGBuilder

getNumberOfThreads
^^^^^^^^^^^^^^^^^^

.. java:method:: public int getNumberOfThreads()
   :outertype: CDGBuilder

getPopulationSize
^^^^^^^^^^^^^^^^^

.. java:method:: public int getPopulationSize()
   :outertype: CDGBuilder

getResultPopulationSize
^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public int getResultPopulationSize()
   :outertype: CDGBuilder

getT
^^^^

.. java:method:: public double getT()
   :outertype: CDGBuilder

setChildGrid
^^^^^^^^^^^^

.. java:method:: public CDGBuilder setChildGrid(int childGrid)
   :outertype: CDGBuilder

setChildGridNum
^^^^^^^^^^^^^^^

.. java:method:: public CDGBuilder setChildGridNum(int childGridNum)
   :outertype: CDGBuilder

setCrossover
^^^^^^^^^^^^

.. java:method:: public CDGBuilder setCrossover(CrossoverOperator<DoubleSolution> crossover)
   :outertype: CDGBuilder

setK
^^^^

.. java:method:: public CDGBuilder setK(int k)
   :outertype: CDGBuilder

setMaxEvaluations
^^^^^^^^^^^^^^^^^

.. java:method:: public CDGBuilder setMaxEvaluations(int maxEvaluations)
   :outertype: CDGBuilder

setNeighborhoodSelectionProbability
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public CDGBuilder setNeighborhoodSelectionProbability(double neighborhoodSelectionProbability)
   :outertype: CDGBuilder

setNumberOfThreads
^^^^^^^^^^^^^^^^^^

.. java:method:: public CDGBuilder setNumberOfThreads(int numberOfThreads)
   :outertype: CDGBuilder

setPopulationSize
^^^^^^^^^^^^^^^^^

.. java:method:: public CDGBuilder setPopulationSize(int populationSize)
   :outertype: CDGBuilder

setResultPopulationSize
^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public CDGBuilder setResultPopulationSize(int resultPopulationSize)
   :outertype: CDGBuilder

setT
^^^^

.. java:method:: public CDGBuilder setT(int t)
   :outertype: CDGBuilder

