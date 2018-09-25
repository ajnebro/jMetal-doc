.. java:import:: org.uma.jmetal.algorithm.impl AbstractEvolutionaryAlgorithm

.. java:import:: org.uma.jmetal.operator CrossoverOperator

.. java:import:: org.uma.jmetal.operator MutationOperator

.. java:import:: org.uma.jmetal.operator SelectionOperator

.. java:import:: org.uma.jmetal.problem BinaryProblem

.. java:import:: org.uma.jmetal.solution BinarySolution

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: org.uma.jmetal.util SolutionListUtils

.. java:import:: org.uma.jmetal.util.archive.impl NonDominatedSolutionListArchive

.. java:import:: org.uma.jmetal.util.binarySet BinarySet

.. java:import:: org.uma.jmetal.util.comparator CrowdingDistanceComparator

.. java:import:: org.uma.jmetal.util.evaluator SolutionListEvaluator

.. java:import:: java.util ArrayList

.. java:import:: java.util Collections

.. java:import:: java.util Comparator

.. java:import:: java.util List

MOCHC
=====

.. java:package:: org.uma.jmetal.algorithm.multiobjective.mochc
   :noindex:

.. java:type:: @SuppressWarnings public class MOCHC extends AbstractEvolutionaryAlgorithm<BinarySolution, List<BinarySolution>>

   This class executes the MOCHC algorithm described in: A.J. Nebro, E. Alba, G. Molina, F. Chicano, F. Luna, J.J. Durillo "Optimal antenna placement using a new multi-objective chc algorithm". GECCO '07: Proceedings of the 9th annual conference on Genetic and evolutionary computation. London, England. July 2007.

Constructors
------------
MOCHC
^^^^^

.. java:constructor:: public MOCHC(BinaryProblem problem, int populationSize, int maxEvaluations, int convergenceValue, double preservedPopulation, double initialConvergenceCount, CrossoverOperator<BinarySolution> crossoverOperator, MutationOperator<BinarySolution> cataclysmicMutation, SelectionOperator<List<BinarySolution>, List<BinarySolution>> newGenerationSelection, SelectionOperator<List<BinarySolution>, BinarySolution> parentSelection, SolutionListEvaluator<BinarySolution> evaluator)
   :outertype: MOCHC

   Constructor

Methods
-------
createInitialPopulation
^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override protected List<BinarySolution> createInitialPopulation()
   :outertype: MOCHC

evaluatePopulation
^^^^^^^^^^^^^^^^^^

.. java:method:: @Override protected List<BinarySolution> evaluatePopulation(List<BinarySolution> population)
   :outertype: MOCHC

getDescription
^^^^^^^^^^^^^^

.. java:method:: @Override public String getDescription()
   :outertype: MOCHC

getMaxPopulationSize
^^^^^^^^^^^^^^^^^^^^

.. java:method:: public int getMaxPopulationSize()
   :outertype: MOCHC

getName
^^^^^^^

.. java:method:: @Override public String getName()
   :outertype: MOCHC

getResult
^^^^^^^^^

.. java:method:: @Override public List<BinarySolution> getResult()
   :outertype: MOCHC

initProgress
^^^^^^^^^^^^

.. java:method:: @Override protected void initProgress()
   :outertype: MOCHC

isStoppingConditionReached
^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override protected boolean isStoppingConditionReached()
   :outertype: MOCHC

replacement
^^^^^^^^^^^

.. java:method:: @Override protected List<BinarySolution> replacement(List<BinarySolution> population, List<BinarySolution> offspringPopulation)
   :outertype: MOCHC

reproduction
^^^^^^^^^^^^

.. java:method:: @Override protected List<BinarySolution> reproduction(List<BinarySolution> matingPopulation)
   :outertype: MOCHC

selection
^^^^^^^^^

.. java:method:: @Override protected List<BinarySolution> selection(List<BinarySolution> population)
   :outertype: MOCHC

setMaxPopulationSize
^^^^^^^^^^^^^^^^^^^^

.. java:method:: public void setMaxPopulationSize(int maxPopulationSize)
   :outertype: MOCHC

updateProgress
^^^^^^^^^^^^^^

.. java:method:: @Override protected void updateProgress()
   :outertype: MOCHC

