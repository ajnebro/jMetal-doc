.. java:import:: org.uma.jmetal.algorithm.impl AbstractDifferentialEvolution

.. java:import:: org.uma.jmetal.operator.impl.crossover DifferentialEvolutionCrossover

.. java:import:: org.uma.jmetal.operator.impl.selection DifferentialEvolutionSelection

.. java:import:: org.uma.jmetal.problem DoubleProblem

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.util.comparator ObjectiveComparator

.. java:import:: org.uma.jmetal.util.evaluator SolutionListEvaluator

.. java:import:: java.util ArrayList

.. java:import:: java.util Collections

.. java:import:: java.util Comparator

.. java:import:: java.util List

DifferentialEvolution
=====================

.. java:package:: org.uma.jmetal.algorithm.singleobjective.differentialevolution
   :noindex:

.. java:type:: @SuppressWarnings public class DifferentialEvolution extends AbstractDifferentialEvolution<DoubleSolution>

   This class implements a differential evolution algorithm.

   :author: Antonio J. Nebro

Constructors
------------
DifferentialEvolution
^^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public DifferentialEvolution(DoubleProblem problem, int maxEvaluations, int populationSize, DifferentialEvolutionCrossover crossoverOperator, DifferentialEvolutionSelection selectionOperator, SolutionListEvaluator<DoubleSolution> evaluator)
   :outertype: DifferentialEvolution

   Constructor

   :param problem: Problem to solve
   :param maxEvaluations: Maximum number of evaluations to perform
   :param populationSize:
   :param crossoverOperator:
   :param selectionOperator:
   :param evaluator:

Methods
-------
createInitialPopulation
^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override protected List<DoubleSolution> createInitialPopulation()
   :outertype: DifferentialEvolution

evaluatePopulation
^^^^^^^^^^^^^^^^^^

.. java:method:: @Override protected List<DoubleSolution> evaluatePopulation(List<DoubleSolution> population)
   :outertype: DifferentialEvolution

getDescription
^^^^^^^^^^^^^^

.. java:method:: @Override public String getDescription()
   :outertype: DifferentialEvolution

getEvaluations
^^^^^^^^^^^^^^

.. java:method:: public int getEvaluations()
   :outertype: DifferentialEvolution

getName
^^^^^^^

.. java:method:: @Override public String getName()
   :outertype: DifferentialEvolution

getResult
^^^^^^^^^

.. java:method:: @Override public DoubleSolution getResult()
   :outertype: DifferentialEvolution

   Returns the best individual

initProgress
^^^^^^^^^^^^

.. java:method:: @Override protected void initProgress()
   :outertype: DifferentialEvolution

isStoppingConditionReached
^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override protected boolean isStoppingConditionReached()
   :outertype: DifferentialEvolution

replacement
^^^^^^^^^^^

.. java:method:: @Override protected List<DoubleSolution> replacement(List<DoubleSolution> population, List<DoubleSolution> offspringPopulation)
   :outertype: DifferentialEvolution

reproduction
^^^^^^^^^^^^

.. java:method:: @Override protected List<DoubleSolution> reproduction(List<DoubleSolution> matingPopulation)
   :outertype: DifferentialEvolution

selection
^^^^^^^^^

.. java:method:: @Override protected List<DoubleSolution> selection(List<DoubleSolution> population)
   :outertype: DifferentialEvolution

setEvaluations
^^^^^^^^^^^^^^

.. java:method:: public void setEvaluations(int evaluations)
   :outertype: DifferentialEvolution

updateProgress
^^^^^^^^^^^^^^

.. java:method:: @Override protected void updateProgress()
   :outertype: DifferentialEvolution

