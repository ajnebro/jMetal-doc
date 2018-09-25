.. java:import:: org.uma.jmetal.algorithm.impl AbstractGeneticAlgorithm

.. java:import:: org.uma.jmetal.algorithm.multiobjective.espea.util EnergyArchive

.. java:import:: org.uma.jmetal.algorithm.multiobjective.espea.util EnergyArchive.ReplacementStrategy

.. java:import:: org.uma.jmetal.algorithm.multiobjective.espea.util ScalarizationWrapper

.. java:import:: org.uma.jmetal.operator CrossoverOperator

.. java:import:: org.uma.jmetal.operator MutationOperator

.. java:import:: org.uma.jmetal.operator SelectionOperator

.. java:import:: org.uma.jmetal.problem Problem

.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util.evaluator SolutionListEvaluator

.. java:import:: java.util ArrayList

.. java:import:: java.util List

ESPEA
=====

.. java:package:: org.uma.jmetal.algorithm.multiobjective.espea
   :noindex:

.. java:type:: @SuppressWarnings public class ESPEA<S extends Solution<?>> extends AbstractGeneticAlgorithm<S, List<S>>

   Implementation of the Electrostatic Potential Energy Evolutionary Algorithm (ESPEA) from the paper "Obtaining Optimal Pareto Front Approximations using Scalarized Preference Information" by M. Braun et al.

   The algorithm generates preference-biased Pareto front approximations that cover the entire front but focus more solutions in those regions that are interesting to the decision maker. Preferences are presented to the algorithm in the form of a scalarization function (value function) that maps the vector of objective to a real value. Smaller values are deemed to indicate higher desirability to comply with minimization.

   If no scalarized preference is specified, uniform preferences are assumed and ESPEA generates a uniform approximation of the Pareto front.

   :author: Marlon Braun

Fields
------
archive
^^^^^^^

.. java:field:: protected final EnergyArchive<S> archive
   :outertype: ESPEA

   An archive of nondominated solutions that approximates the energy minimum state based on the chosen scalarization function.

evaluations
^^^^^^^^^^^

.. java:field:: protected int evaluations
   :outertype: ESPEA

   The number of function evaluations that have been executed so far.

evaluator
^^^^^^^^^

.. java:field:: protected final SolutionListEvaluator<S> evaluator
   :outertype: ESPEA

   Evaluates the solutions

fullArchiveCrossoverOperator
^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:field:: protected CrossoverOperator<S> fullArchiveCrossoverOperator
   :outertype: ESPEA

   ESPEA uses two different crossover operators depending on the current archive size. If the archive is not full, it uses the crossover operator provided by \ :java:ref:`getCrossoverOperator()`\ . If the archive is full, \ :java:ref:`fullArchiveCrossoverOperator`\  is used.

maxEvaluations
^^^^^^^^^^^^^^

.. java:field:: protected int maxEvaluations
   :outertype: ESPEA

   Maximum number of functions evaluations that are executed.

Constructors
------------
ESPEA
^^^^^

.. java:constructor:: public ESPEA(Problem<S> problem, int maxEvaluations, int populationSize, CrossoverOperator<S> crossoverOperator, CrossoverOperator<S> fullArchiveCrossoverOperator, MutationOperator<S> mutationOperator, SelectionOperator<List<S>, S> selectionOperator, ScalarizationWrapper scalarizationWrapper, SolutionListEvaluator<S> evaluator, boolean normalizeObjectives, ReplacementStrategy replacementStrategy)
   :outertype: ESPEA

   Constructor for setting all parameters of ESPEA.

Methods
-------
evaluatePopulation
^^^^^^^^^^^^^^^^^^

.. java:method:: @Override protected List<S> evaluatePopulation(List<S> population)
   :outertype: ESPEA

getDescription
^^^^^^^^^^^^^^

.. java:method:: @Override public String getDescription()
   :outertype: ESPEA

getName
^^^^^^^

.. java:method:: @Override public String getName()
   :outertype: ESPEA

getResult
^^^^^^^^^

.. java:method:: @Override public List<S> getResult()
   :outertype: ESPEA

initProgress
^^^^^^^^^^^^

.. java:method:: @Override protected void initProgress()
   :outertype: ESPEA

isStoppingConditionReached
^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override protected boolean isStoppingConditionReached()
   :outertype: ESPEA

replacement
^^^^^^^^^^^

.. java:method:: @Override protected List<S> replacement(List<S> population, List<S> offspringPopulation)
   :outertype: ESPEA

reproduction
^^^^^^^^^^^^

.. java:method:: @Override protected List<S> reproduction(List<S> population)
   :outertype: ESPEA

selection
^^^^^^^^^

.. java:method:: @Override protected List<S> selection(List<S> population)
   :outertype: ESPEA

updateProgress
^^^^^^^^^^^^^^

.. java:method:: @Override protected void updateProgress()
   :outertype: ESPEA

