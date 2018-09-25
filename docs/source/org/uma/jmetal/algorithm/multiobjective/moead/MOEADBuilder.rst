.. java:import:: org.uma.jmetal.operator CrossoverOperator

.. java:import:: org.uma.jmetal.operator MutationOperator

.. java:import:: org.uma.jmetal.operator.impl.crossover DifferentialEvolutionCrossover

.. java:import:: org.uma.jmetal.operator.impl.mutation PolynomialMutation

.. java:import:: org.uma.jmetal.problem Problem

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.util AlgorithmBuilder

MOEADBuilder
============

.. java:package:: org.uma.jmetal.algorithm.multiobjective.moead
   :noindex:

.. java:type:: public class MOEADBuilder implements AlgorithmBuilder<AbstractMOEAD<DoubleSolution>>

   Builder class for algorithm MOEA/D and variants

   :author: Antonio J. Nebro

Fields
------
crossover
^^^^^^^^^

.. java:field:: protected CrossoverOperator<DoubleSolution> crossover
   :outertype: MOEADBuilder

dataDirectory
^^^^^^^^^^^^^

.. java:field:: protected String dataDirectory
   :outertype: MOEADBuilder

functionType
^^^^^^^^^^^^

.. java:field:: protected MOEAD.FunctionType functionType
   :outertype: MOEADBuilder

maxEvaluations
^^^^^^^^^^^^^^

.. java:field:: protected int maxEvaluations
   :outertype: MOEADBuilder

maximumNumberOfReplacedSolutions
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:field:: protected int maximumNumberOfReplacedSolutions
   :outertype: MOEADBuilder

   nr in Zhang & Li paper

moeadVariant
^^^^^^^^^^^^

.. java:field:: protected Variant moeadVariant
   :outertype: MOEADBuilder

mutation
^^^^^^^^

.. java:field:: protected MutationOperator<DoubleSolution> mutation
   :outertype: MOEADBuilder

neighborSize
^^^^^^^^^^^^

.. java:field:: protected int neighborSize
   :outertype: MOEADBuilder

   T in Zhang & Li paper

neighborhoodSelectionProbability
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:field:: protected double neighborhoodSelectionProbability
   :outertype: MOEADBuilder

   Delta in Zhang & Li paper

numberOfThreads
^^^^^^^^^^^^^^^

.. java:field:: protected int numberOfThreads
   :outertype: MOEADBuilder

populationSize
^^^^^^^^^^^^^^

.. java:field:: protected int populationSize
   :outertype: MOEADBuilder

problem
^^^^^^^

.. java:field:: protected Problem<DoubleSolution> problem
   :outertype: MOEADBuilder

resultPopulationSize
^^^^^^^^^^^^^^^^^^^^

.. java:field:: protected int resultPopulationSize
   :outertype: MOEADBuilder

Constructors
------------
MOEADBuilder
^^^^^^^^^^^^

.. java:constructor:: public MOEADBuilder(Problem<DoubleSolution> problem, Variant variant)
   :outertype: MOEADBuilder

   Constructor

Methods
-------
build
^^^^^

.. java:method:: public AbstractMOEAD<DoubleSolution> build()
   :outertype: MOEADBuilder

getCrossover
^^^^^^^^^^^^

.. java:method:: public CrossoverOperator<DoubleSolution> getCrossover()
   :outertype: MOEADBuilder

getDataDirectory
^^^^^^^^^^^^^^^^

.. java:method:: public String getDataDirectory()
   :outertype: MOEADBuilder

getFunctionType
^^^^^^^^^^^^^^^

.. java:method:: public MOEAD.FunctionType getFunctionType()
   :outertype: MOEADBuilder

getMaxEvaluations
^^^^^^^^^^^^^^^^^

.. java:method:: public int getMaxEvaluations()
   :outertype: MOEADBuilder

getMaximumNumberOfReplacedSolutions
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public int getMaximumNumberOfReplacedSolutions()
   :outertype: MOEADBuilder

getMutation
^^^^^^^^^^^

.. java:method:: public MutationOperator<DoubleSolution> getMutation()
   :outertype: MOEADBuilder

getNeighborSize
^^^^^^^^^^^^^^^

.. java:method:: public int getNeighborSize()
   :outertype: MOEADBuilder

getNeighborhoodSelectionProbability
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public double getNeighborhoodSelectionProbability()
   :outertype: MOEADBuilder

getNumberOfThreads
^^^^^^^^^^^^^^^^^^

.. java:method:: public int getNumberOfThreads()
   :outertype: MOEADBuilder

getPopulationSize
^^^^^^^^^^^^^^^^^

.. java:method:: public int getPopulationSize()
   :outertype: MOEADBuilder

getResultPopulationSize
^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public int getResultPopulationSize()
   :outertype: MOEADBuilder

setCrossover
^^^^^^^^^^^^

.. java:method:: public MOEADBuilder setCrossover(CrossoverOperator<DoubleSolution> crossover)
   :outertype: MOEADBuilder

setDataDirectory
^^^^^^^^^^^^^^^^

.. java:method:: public MOEADBuilder setDataDirectory(String dataDirectory)
   :outertype: MOEADBuilder

setFunctionType
^^^^^^^^^^^^^^^

.. java:method:: public MOEADBuilder setFunctionType(MOEAD.FunctionType functionType)
   :outertype: MOEADBuilder

setMaxEvaluations
^^^^^^^^^^^^^^^^^

.. java:method:: public MOEADBuilder setMaxEvaluations(int maxEvaluations)
   :outertype: MOEADBuilder

setMaximumNumberOfReplacedSolutions
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public MOEADBuilder setMaximumNumberOfReplacedSolutions(int maximumNumberOfReplacedSolutions)
   :outertype: MOEADBuilder

setMutation
^^^^^^^^^^^

.. java:method:: public MOEADBuilder setMutation(MutationOperator<DoubleSolution> mutation)
   :outertype: MOEADBuilder

setNeighborSize
^^^^^^^^^^^^^^^

.. java:method:: public MOEADBuilder setNeighborSize(int neighborSize)
   :outertype: MOEADBuilder

setNeighborhoodSelectionProbability
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public MOEADBuilder setNeighborhoodSelectionProbability(double neighborhoodSelectionProbability)
   :outertype: MOEADBuilder

setNumberOfThreads
^^^^^^^^^^^^^^^^^^

.. java:method:: public MOEADBuilder setNumberOfThreads(int numberOfThreads)
   :outertype: MOEADBuilder

setPopulationSize
^^^^^^^^^^^^^^^^^

.. java:method:: public MOEADBuilder setPopulationSize(int populationSize)
   :outertype: MOEADBuilder

setResultPopulationSize
^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public MOEADBuilder setResultPopulationSize(int resultPopulationSize)
   :outertype: MOEADBuilder

