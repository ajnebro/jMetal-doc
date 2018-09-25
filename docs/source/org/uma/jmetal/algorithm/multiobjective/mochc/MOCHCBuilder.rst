.. java:import:: org.uma.jmetal.operator CrossoverOperator

.. java:import:: org.uma.jmetal.operator MutationOperator

.. java:import:: org.uma.jmetal.operator SelectionOperator

.. java:import:: org.uma.jmetal.problem BinaryProblem

.. java:import:: org.uma.jmetal.solution BinarySolution

.. java:import:: org.uma.jmetal.util AlgorithmBuilder

.. java:import:: org.uma.jmetal.util.evaluator SolutionListEvaluator

.. java:import:: org.uma.jmetal.util.evaluator.impl SequentialSolutionListEvaluator

.. java:import:: java.util List

MOCHCBuilder
============

.. java:package:: org.uma.jmetal.algorithm.multiobjective.mochc
   :noindex:

.. java:type:: public class MOCHCBuilder implements AlgorithmBuilder<MOCHC>

   Builder class

Fields
------
cataclysmicMutation
^^^^^^^^^^^^^^^^^^^

.. java:field::  MutationOperator<BinarySolution> cataclysmicMutation
   :outertype: MOCHCBuilder

convergenceValue
^^^^^^^^^^^^^^^^

.. java:field::  int convergenceValue
   :outertype: MOCHCBuilder

crossoverOperator
^^^^^^^^^^^^^^^^^

.. java:field::  CrossoverOperator<BinarySolution> crossoverOperator
   :outertype: MOCHCBuilder

evaluator
^^^^^^^^^

.. java:field::  SolutionListEvaluator<BinarySolution> evaluator
   :outertype: MOCHCBuilder

initialConvergenceCount
^^^^^^^^^^^^^^^^^^^^^^^

.. java:field::  double initialConvergenceCount
   :outertype: MOCHCBuilder

maxEvaluations
^^^^^^^^^^^^^^

.. java:field::  int maxEvaluations
   :outertype: MOCHCBuilder

newGenerationSelection
^^^^^^^^^^^^^^^^^^^^^^

.. java:field::  SelectionOperator<List<BinarySolution>, List<BinarySolution>> newGenerationSelection
   :outertype: MOCHCBuilder

parentSelection
^^^^^^^^^^^^^^^

.. java:field::  SelectionOperator<List<BinarySolution>, BinarySolution> parentSelection
   :outertype: MOCHCBuilder

populationSize
^^^^^^^^^^^^^^

.. java:field::  int populationSize
   :outertype: MOCHCBuilder

preservedPopulation
^^^^^^^^^^^^^^^^^^^

.. java:field::  double preservedPopulation
   :outertype: MOCHCBuilder

problem
^^^^^^^

.. java:field::  BinaryProblem problem
   :outertype: MOCHCBuilder

Constructors
------------
MOCHCBuilder
^^^^^^^^^^^^

.. java:constructor:: public MOCHCBuilder(BinaryProblem problem)
   :outertype: MOCHCBuilder

Methods
-------
build
^^^^^

.. java:method:: public MOCHC build()
   :outertype: MOCHCBuilder

getCataclysmicMutation
^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public MutationOperator<BinarySolution> getCataclysmicMutation()
   :outertype: MOCHCBuilder

getConvergenceValue
^^^^^^^^^^^^^^^^^^^

.. java:method:: public int getConvergenceValue()
   :outertype: MOCHCBuilder

getCrossover
^^^^^^^^^^^^

.. java:method:: public CrossoverOperator<BinarySolution> getCrossover()
   :outertype: MOCHCBuilder

getInitialConvergenceCount
^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public double getInitialConvergenceCount()
   :outertype: MOCHCBuilder

getMaxEvaluation
^^^^^^^^^^^^^^^^

.. java:method:: public int getMaxEvaluation()
   :outertype: MOCHCBuilder

getNewGenerationSelection
^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public SelectionOperator<List<BinarySolution>, List<BinarySolution>> getNewGenerationSelection()
   :outertype: MOCHCBuilder

getParentSelection
^^^^^^^^^^^^^^^^^^

.. java:method:: public SelectionOperator<List<BinarySolution>, BinarySolution> getParentSelection()
   :outertype: MOCHCBuilder

getPopulationSize
^^^^^^^^^^^^^^^^^

.. java:method:: public int getPopulationSize()
   :outertype: MOCHCBuilder

getPreservedPopulation
^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public double getPreservedPopulation()
   :outertype: MOCHCBuilder

getProblem
^^^^^^^^^^

.. java:method:: public BinaryProblem getProblem()
   :outertype: MOCHCBuilder

setCataclysmicMutation
^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public MOCHCBuilder setCataclysmicMutation(MutationOperator<BinarySolution> cataclysmicMutation)
   :outertype: MOCHCBuilder

setConvergenceValue
^^^^^^^^^^^^^^^^^^^

.. java:method:: public MOCHCBuilder setConvergenceValue(int convergenceValue)
   :outertype: MOCHCBuilder

setCrossover
^^^^^^^^^^^^

.. java:method:: public MOCHCBuilder setCrossover(CrossoverOperator<BinarySolution> crossover)
   :outertype: MOCHCBuilder

setEvaluator
^^^^^^^^^^^^

.. java:method:: public MOCHCBuilder setEvaluator(SolutionListEvaluator<BinarySolution> evaluator)
   :outertype: MOCHCBuilder

setInitialConvergenceCount
^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public MOCHCBuilder setInitialConvergenceCount(double initialConvergenceCount)
   :outertype: MOCHCBuilder

setMaxEvaluations
^^^^^^^^^^^^^^^^^

.. java:method:: public MOCHCBuilder setMaxEvaluations(int maxEvaluations)
   :outertype: MOCHCBuilder

setNewGenerationSelection
^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public MOCHCBuilder setNewGenerationSelection(SelectionOperator<List<BinarySolution>, List<BinarySolution>> newGenerationSelection)
   :outertype: MOCHCBuilder

setParentSelection
^^^^^^^^^^^^^^^^^^

.. java:method:: public MOCHCBuilder setParentSelection(SelectionOperator<List<BinarySolution>, BinarySolution> parentSelection)
   :outertype: MOCHCBuilder

setPopulationSize
^^^^^^^^^^^^^^^^^

.. java:method:: public MOCHCBuilder setPopulationSize(int populationSize)
   :outertype: MOCHCBuilder

setPreservedPopulation
^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public MOCHCBuilder setPreservedPopulation(double preservedPopulation)
   :outertype: MOCHCBuilder

