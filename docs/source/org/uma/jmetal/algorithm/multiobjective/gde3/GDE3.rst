.. java:import:: org.uma.jmetal.algorithm.impl AbstractDifferentialEvolution

.. java:import:: org.uma.jmetal.operator.impl.crossover DifferentialEvolutionCrossover

.. java:import:: org.uma.jmetal.operator.impl.selection DifferentialEvolutionSelection

.. java:import:: org.uma.jmetal.problem DoubleProblem

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.util SolutionListUtils

.. java:import:: org.uma.jmetal.util.comparator CrowdingDistanceComparator

.. java:import:: org.uma.jmetal.util.comparator DominanceComparator

.. java:import:: org.uma.jmetal.util.evaluator SolutionListEvaluator

.. java:import:: org.uma.jmetal.util.solutionattribute DensityEstimator

.. java:import:: org.uma.jmetal.util.solutionattribute Ranking

.. java:import:: org.uma.jmetal.util.solutionattribute.impl CrowdingDistance

.. java:import:: org.uma.jmetal.util.solutionattribute.impl DominanceRanking

GDE3
====

.. java:package:: org.uma.jmetal.algorithm.multiobjective.gde3
   :noindex:

.. java:type:: @SuppressWarnings public class GDE3 extends AbstractDifferentialEvolution<List<DoubleSolution>>

   This class implements the GDE3 algorithm

Fields
------
crowdingDistance
^^^^^^^^^^^^^^^^

.. java:field:: protected DensityEstimator<DoubleSolution> crowdingDistance
   :outertype: GDE3

dominanceComparator
^^^^^^^^^^^^^^^^^^^

.. java:field:: protected Comparator<DoubleSolution> dominanceComparator
   :outertype: GDE3

evaluations
^^^^^^^^^^^

.. java:field:: protected int evaluations
   :outertype: GDE3

evaluator
^^^^^^^^^

.. java:field:: protected SolutionListEvaluator<DoubleSolution> evaluator
   :outertype: GDE3

maxEvaluations
^^^^^^^^^^^^^^

.. java:field:: protected int maxEvaluations
   :outertype: GDE3

ranking
^^^^^^^

.. java:field:: protected Ranking<DoubleSolution> ranking
   :outertype: GDE3

Constructors
------------
GDE3
^^^^

.. java:constructor:: public GDE3(DoubleProblem problem, int populationSize, int maxEvaluations, DifferentialEvolutionSelection selection, DifferentialEvolutionCrossover crossover, SolutionListEvaluator<DoubleSolution> evaluator)
   :outertype: GDE3

   Constructor

Methods
-------
addLastRankedSolutionsToPopulation
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: protected void addLastRankedSolutionsToPopulation(Ranking<DoubleSolution> ranking, int rank, List<DoubleSolution> population)
   :outertype: GDE3

addRankedSolutionsToPopulation
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: protected void addRankedSolutionsToPopulation(Ranking<DoubleSolution> ranking, int rank, List<DoubleSolution> population)
   :outertype: GDE3

computeRanking
^^^^^^^^^^^^^^

.. java:method:: protected Ranking<DoubleSolution> computeRanking(List<DoubleSolution> solutionList)
   :outertype: GDE3

createInitialPopulation
^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override protected List<DoubleSolution> createInitialPopulation()
   :outertype: GDE3

crowdingDistanceSelection
^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: protected List<DoubleSolution> crowdingDistanceSelection(Ranking<DoubleSolution> ranking)
   :outertype: GDE3

evaluatePopulation
^^^^^^^^^^^^^^^^^^

.. java:method:: @Override protected List<DoubleSolution> evaluatePopulation(List<DoubleSolution> population)
   :outertype: GDE3

   Evaluate population method

   :param population: The list of solutions to be evaluated
   :return: A list of evaluated solutions

getDescription
^^^^^^^^^^^^^^

.. java:method:: @Override public String getDescription()
   :outertype: GDE3

getMaxPopulationSize
^^^^^^^^^^^^^^^^^^^^

.. java:method:: public int getMaxPopulationSize()
   :outertype: GDE3

getName
^^^^^^^

.. java:method:: @Override public String getName()
   :outertype: GDE3

getNonDominatedSolutions
^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: protected List<DoubleSolution> getNonDominatedSolutions(List<DoubleSolution> solutionList)
   :outertype: GDE3

getResult
^^^^^^^^^

.. java:method:: @Override public List<DoubleSolution> getResult()
   :outertype: GDE3

initProgress
^^^^^^^^^^^^

.. java:method:: @Override protected void initProgress()
   :outertype: GDE3

isStoppingConditionReached
^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override protected boolean isStoppingConditionReached()
   :outertype: GDE3

populationIsNotFull
^^^^^^^^^^^^^^^^^^^

.. java:method:: protected boolean populationIsNotFull(List<DoubleSolution> population)
   :outertype: GDE3

replacement
^^^^^^^^^^^

.. java:method:: @Override protected List<DoubleSolution> replacement(List<DoubleSolution> population, List<DoubleSolution> offspringPopulation)
   :outertype: GDE3

reproduction
^^^^^^^^^^^^

.. java:method:: @Override protected List<DoubleSolution> reproduction(List<DoubleSolution> matingPopulation)
   :outertype: GDE3

selection
^^^^^^^^^

.. java:method:: @Override protected List<DoubleSolution> selection(List<DoubleSolution> population)
   :outertype: GDE3

setMaxPopulationSize
^^^^^^^^^^^^^^^^^^^^

.. java:method:: public void setMaxPopulationSize(int maxPopulationSize)
   :outertype: GDE3

subfrontFillsIntoThePopulation
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: protected boolean subfrontFillsIntoThePopulation(Ranking<DoubleSolution> ranking, int rank, List<DoubleSolution> population)
   :outertype: GDE3

updateProgress
^^^^^^^^^^^^^^

.. java:method:: @Override protected void updateProgress()
   :outertype: GDE3

