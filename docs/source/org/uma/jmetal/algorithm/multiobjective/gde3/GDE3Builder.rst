.. java:import:: org.uma.jmetal.operator CrossoverOperator

.. java:import:: org.uma.jmetal.operator SelectionOperator

.. java:import:: org.uma.jmetal.operator.impl.crossover DifferentialEvolutionCrossover

.. java:import:: org.uma.jmetal.operator.impl.selection DifferentialEvolutionSelection

.. java:import:: org.uma.jmetal.problem DoubleProblem

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.util AlgorithmBuilder

.. java:import:: org.uma.jmetal.util.evaluator SolutionListEvaluator

.. java:import:: org.uma.jmetal.util.evaluator.impl SequentialSolutionListEvaluator

.. java:import:: java.util List

GDE3Builder
===========

.. java:package:: org.uma.jmetal.algorithm.multiobjective.gde3
   :noindex:

.. java:type:: public class GDE3Builder implements AlgorithmBuilder<GDE3>

   This class implements the GDE3 algorithm

Fields
------
crossoverOperator
^^^^^^^^^^^^^^^^^

.. java:field:: protected DifferentialEvolutionCrossover crossoverOperator
   :outertype: GDE3Builder

evaluator
^^^^^^^^^

.. java:field:: protected SolutionListEvaluator<DoubleSolution> evaluator
   :outertype: GDE3Builder

maxEvaluations
^^^^^^^^^^^^^^

.. java:field:: protected int maxEvaluations
   :outertype: GDE3Builder

populationSize
^^^^^^^^^^^^^^

.. java:field:: protected int populationSize
   :outertype: GDE3Builder

selectionOperator
^^^^^^^^^^^^^^^^^

.. java:field:: protected DifferentialEvolutionSelection selectionOperator
   :outertype: GDE3Builder

Constructors
------------
GDE3Builder
^^^^^^^^^^^

.. java:constructor:: public GDE3Builder(DoubleProblem problem)
   :outertype: GDE3Builder

   Constructor

Methods
-------
build
^^^^^

.. java:method:: public GDE3 build()
   :outertype: GDE3Builder

getCrossoverOperator
^^^^^^^^^^^^^^^^^^^^

.. java:method:: public CrossoverOperator<DoubleSolution> getCrossoverOperator()
   :outertype: GDE3Builder

getMaxEvaluations
^^^^^^^^^^^^^^^^^

.. java:method:: public int getMaxEvaluations()
   :outertype: GDE3Builder

getPopulationSize
^^^^^^^^^^^^^^^^^

.. java:method:: public int getPopulationSize()
   :outertype: GDE3Builder

getSelectionOperator
^^^^^^^^^^^^^^^^^^^^

.. java:method:: public SelectionOperator<List<DoubleSolution>, List<DoubleSolution>> getSelectionOperator()
   :outertype: GDE3Builder

setCrossover
^^^^^^^^^^^^

.. java:method:: public GDE3Builder setCrossover(DifferentialEvolutionCrossover crossover)
   :outertype: GDE3Builder

setMaxEvaluations
^^^^^^^^^^^^^^^^^

.. java:method:: public GDE3Builder setMaxEvaluations(int maxEvaluations)
   :outertype: GDE3Builder

setPopulationSize
^^^^^^^^^^^^^^^^^

.. java:method:: public GDE3Builder setPopulationSize(int populationSize)
   :outertype: GDE3Builder

setSelection
^^^^^^^^^^^^

.. java:method:: public GDE3Builder setSelection(DifferentialEvolutionSelection selection)
   :outertype: GDE3Builder

setSolutionSetEvaluator
^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public GDE3Builder setSolutionSetEvaluator(SolutionListEvaluator<DoubleSolution> evaluator)
   :outertype: GDE3Builder

