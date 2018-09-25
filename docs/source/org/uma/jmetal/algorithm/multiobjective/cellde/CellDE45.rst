.. java:import:: org.uma.jmetal.algorithm Algorithm

.. java:import:: org.uma.jmetal.operator SelectionOperator

.. java:import:: org.uma.jmetal.operator.impl.crossover DifferentialEvolutionCrossover

.. java:import:: org.uma.jmetal.problem Problem

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.util.archive BoundedArchive

.. java:import:: org.uma.jmetal.util.comparator CrowdingDistanceComparator

.. java:import:: org.uma.jmetal.util.comparator DominanceComparator

.. java:import:: org.uma.jmetal.util.evaluator SolutionListEvaluator

.. java:import:: org.uma.jmetal.util.neighborhood Neighborhood

.. java:import:: org.uma.jmetal.util.pseudorandom JMetalRandom

.. java:import:: org.uma.jmetal.util.solutionattribute Ranking

.. java:import:: org.uma.jmetal.util.solutionattribute.impl CrowdingDistance

.. java:import:: org.uma.jmetal.util.solutionattribute.impl DominanceRanking

.. java:import:: org.uma.jmetal.util.solutionattribute.impl LocationAttribute

.. java:import:: java.util ArrayList

.. java:import:: java.util Comparator

.. java:import:: java.util List

CellDE45
========

.. java:package:: org.uma.jmetal.algorithm.multiobjective.cellde
   :noindex:

.. java:type:: @SuppressWarnings public class CellDE45 implements Algorithm<List<DoubleSolution>>

   :author: Antonio J. Nebro

Fields
------
evaluations
^^^^^^^^^^^

.. java:field:: protected int evaluations
   :outertype: CellDE45

maxEvaluations
^^^^^^^^^^^^^^

.. java:field:: protected int maxEvaluations
   :outertype: CellDE45

Constructors
------------
CellDE45
^^^^^^^^

.. java:constructor:: public CellDE45(Problem<DoubleSolution> problem, int maxEvaluations, int populationSize, BoundedArchive<DoubleSolution> archive, Neighborhood<DoubleSolution> neighborhood, SelectionOperator<List<DoubleSolution>, DoubleSolution> selection, DifferentialEvolutionCrossover crossover, double feedback, SolutionListEvaluator<DoubleSolution> evaluator)
   :outertype: CellDE45

Methods
-------
computeRanking
^^^^^^^^^^^^^^

.. java:method:: protected Ranking<DoubleSolution> computeRanking(List<DoubleSolution> solutionList)
   :outertype: CellDE45

createInitialPopulation
^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: protected List<DoubleSolution> createInitialPopulation()
   :outertype: CellDE45

evaluatePopulation
^^^^^^^^^^^^^^^^^^

.. java:method:: protected List<DoubleSolution> evaluatePopulation(List<DoubleSolution> population)
   :outertype: CellDE45

getDescription
^^^^^^^^^^^^^^

.. java:method:: @Override public String getDescription()
   :outertype: CellDE45

getName
^^^^^^^

.. java:method:: @Override public String getName()
   :outertype: CellDE45

getResult
^^^^^^^^^

.. java:method:: @Override public List<DoubleSolution> getResult()
   :outertype: CellDE45

initProgress
^^^^^^^^^^^^

.. java:method:: protected void initProgress()
   :outertype: CellDE45

isStoppingConditionReached
^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: protected boolean isStoppingConditionReached()
   :outertype: CellDE45

run
^^^

.. java:method:: @Override public void run()
   :outertype: CellDE45

updateProgress
^^^^^^^^^^^^^^

.. java:method:: protected void updateProgress()
   :outertype: CellDE45

