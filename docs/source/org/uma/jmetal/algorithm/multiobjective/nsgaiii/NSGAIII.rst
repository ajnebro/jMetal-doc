.. java:import:: org.uma.jmetal.algorithm.impl AbstractGeneticAlgorithm

.. java:import:: org.uma.jmetal.algorithm.multiobjective.nsgaiii.util EnvironmentalSelection

.. java:import:: org.uma.jmetal.algorithm.multiobjective.nsgaiii.util ReferencePoint

.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util JMetalLogger

.. java:import:: org.uma.jmetal.util SolutionListUtils

.. java:import:: org.uma.jmetal.util.evaluator SolutionListEvaluator

.. java:import:: org.uma.jmetal.util.solutionattribute Ranking

.. java:import:: org.uma.jmetal.util.solutionattribute.impl DominanceRanking

.. java:import:: java.util ArrayList

.. java:import:: java.util List

.. java:import:: java.util Vector

NSGAIII
=======

.. java:package:: org.uma.jmetal.algorithm.multiobjective.nsgaiii
   :noindex:

.. java:type:: @SuppressWarnings public class NSGAIII<S extends Solution<?>> extends AbstractGeneticAlgorithm<S, List<S>>

   Created by ajnebro on 30/10/14. Modified by Juanjo on 13/11/14 This implementation is based on the code of Tsung-Che Chiang http://web.ntnu.edu.tw/~tcchiang/publications/nsga3cpp/nsga3cpp.htm

Fields
------
evaluator
^^^^^^^^^

.. java:field:: protected SolutionListEvaluator<S> evaluator
   :outertype: NSGAIII

iterations
^^^^^^^^^^

.. java:field:: protected int iterations
   :outertype: NSGAIII

maxIterations
^^^^^^^^^^^^^

.. java:field:: protected int maxIterations
   :outertype: NSGAIII

numberOfDivisions
^^^^^^^^^^^^^^^^^

.. java:field:: protected Vector<Integer> numberOfDivisions
   :outertype: NSGAIII

referencePoints
^^^^^^^^^^^^^^^

.. java:field:: protected List<ReferencePoint<S>> referencePoints
   :outertype: NSGAIII

Constructors
------------
NSGAIII
^^^^^^^

.. java:constructor:: public NSGAIII(NSGAIIIBuilder<S> builder)
   :outertype: NSGAIII

   Constructor

Methods
-------
addRankedSolutionsToPopulation
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: protected void addRankedSolutionsToPopulation(Ranking<S> ranking, int rank, List<S> population)
   :outertype: NSGAIII

computeRanking
^^^^^^^^^^^^^^

.. java:method:: protected Ranking<S> computeRanking(List<S> solutionList)
   :outertype: NSGAIII

evaluatePopulation
^^^^^^^^^^^^^^^^^^

.. java:method:: @Override protected List<S> evaluatePopulation(List<S> population)
   :outertype: NSGAIII

getDescription
^^^^^^^^^^^^^^

.. java:method:: @Override public String getDescription()
   :outertype: NSGAIII

getName
^^^^^^^

.. java:method:: @Override public String getName()
   :outertype: NSGAIII

getNonDominatedSolutions
^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: protected List<S> getNonDominatedSolutions(List<S> solutionList)
   :outertype: NSGAIII

getResult
^^^^^^^^^

.. java:method:: @Override public List<S> getResult()
   :outertype: NSGAIII

initProgress
^^^^^^^^^^^^

.. java:method:: @Override protected void initProgress()
   :outertype: NSGAIII

isStoppingConditionReached
^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override protected boolean isStoppingConditionReached()
   :outertype: NSGAIII

replacement
^^^^^^^^^^^

.. java:method:: @Override protected List<S> replacement(List<S> population, List<S> offspringPopulation)
   :outertype: NSGAIII

reproduction
^^^^^^^^^^^^

.. java:method:: @Override protected List<S> reproduction(List<S> population)
   :outertype: NSGAIII

selection
^^^^^^^^^

.. java:method:: @Override protected List<S> selection(List<S> population)
   :outertype: NSGAIII

updateProgress
^^^^^^^^^^^^^^

.. java:method:: @Override protected void updateProgress()
   :outertype: NSGAIII

