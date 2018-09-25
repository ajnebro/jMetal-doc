.. java:import:: org.uma.jmetal.algorithm.impl AbstractCoralReefsOptimization

.. java:import:: org.uma.jmetal.operator CrossoverOperator

.. java:import:: org.uma.jmetal.operator MutationOperator

.. java:import:: org.uma.jmetal.operator SelectionOperator

.. java:import:: org.uma.jmetal.problem Problem

.. java:import:: org.uma.jmetal.util.pseudorandom.impl MersenneTwisterGenerator

.. java:import:: java.util ArrayList

.. java:import:: java.util Collections

.. java:import:: java.util Comparator

.. java:import:: java.util List

CoralReefsOptimization
======================

.. java:package:: org.uma.jmetal.algorithm.singleobjective.coralreefsoptimization
   :noindex:

.. java:type:: public class CoralReefsOptimization<S> extends AbstractCoralReefsOptimization<S, List<S>>

   :author: Inacio Medeiros

Constructors
------------
CoralReefsOptimization
^^^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public CoralReefsOptimization(Problem<S> problem, int maxEvaluations, Comparator<S> comparator, SelectionOperator<List<S>, S> selectionOperator, CrossoverOperator<S> crossoverOperator, MutationOperator<S> mutationOperator, int n, int m, double rho, double fbs, double fa, double pd, int attemptsToSettle)
   :outertype: CoralReefsOptimization

Methods
-------
asexualReproduction
^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override protected List<S> asexualReproduction(List<S> brooders)
   :outertype: CoralReefsOptimization

createInitialPopulation
^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override protected List<S> createInitialPopulation()
   :outertype: CoralReefsOptimization

depredation
^^^^^^^^^^^

.. java:method:: @Override protected List<S> depredation(List<S> population, List<Coordinate> coordinates)
   :outertype: CoralReefsOptimization

evaluatePopulation
^^^^^^^^^^^^^^^^^^

.. java:method:: @Override protected List<S> evaluatePopulation(List<S> population)
   :outertype: CoralReefsOptimization

generateCoordinates
^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override protected List<Coordinate> generateCoordinates()
   :outertype: CoralReefsOptimization

getDescription
^^^^^^^^^^^^^^

.. java:method:: @Override public String getDescription()
   :outertype: CoralReefsOptimization

getName
^^^^^^^

.. java:method:: @Override public String getName()
   :outertype: CoralReefsOptimization

getResult
^^^^^^^^^

.. java:method:: @Override public List<S> getResult()
   :outertype: CoralReefsOptimization

initProgress
^^^^^^^^^^^^

.. java:method:: @Override protected void initProgress()
   :outertype: CoralReefsOptimization

isStoppingConditionReached
^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override protected boolean isStoppingConditionReached()
   :outertype: CoralReefsOptimization

larvaeSettlementPhase
^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override protected List<S> larvaeSettlementPhase(List<S> larvae, List<S> population, List<Coordinate> coordinates)
   :outertype: CoralReefsOptimization

selectBroadcastSpawners
^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override protected List<S> selectBroadcastSpawners(List<S> population)
   :outertype: CoralReefsOptimization

sexualReproduction
^^^^^^^^^^^^^^^^^^

.. java:method:: @Override protected List<S> sexualReproduction(List<S> broadcastSpawners)
   :outertype: CoralReefsOptimization

updateProgress
^^^^^^^^^^^^^^

.. java:method:: @Override protected void updateProgress()
   :outertype: CoralReefsOptimization

