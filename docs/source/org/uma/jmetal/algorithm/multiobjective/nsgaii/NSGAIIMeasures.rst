.. java:import:: org.uma.jmetal.measure Measurable

.. java:import:: org.uma.jmetal.measure MeasureManager

.. java:import:: org.uma.jmetal.measure.impl BasicMeasure

.. java:import:: org.uma.jmetal.measure.impl CountingMeasure

.. java:import:: org.uma.jmetal.measure.impl DurationMeasure

.. java:import:: org.uma.jmetal.measure.impl SimpleMeasureManager

.. java:import:: org.uma.jmetal.operator CrossoverOperator

.. java:import:: org.uma.jmetal.operator MutationOperator

.. java:import:: org.uma.jmetal.operator SelectionOperator

.. java:import:: org.uma.jmetal.problem Problem

.. java:import:: org.uma.jmetal.qualityindicator.impl.hypervolume PISAHypervolume

.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util.evaluator SolutionListEvaluator

.. java:import:: org.uma.jmetal.util.front Front

.. java:import:: org.uma.jmetal.util.front.imp ArrayFront

.. java:import:: org.uma.jmetal.util.solutionattribute Ranking

.. java:import:: org.uma.jmetal.util.solutionattribute.impl DominanceRanking

.. java:import:: java.util Comparator

.. java:import:: java.util List

NSGAIIMeasures
==============

.. java:package:: org.uma.jmetal.algorithm.multiobjective.nsgaii
   :noindex:

.. java:type:: @SuppressWarnings public class NSGAIIMeasures<S extends Solution<?>> extends NSGAII<S> implements Measurable

   :author: Antonio J. Nebro

Fields
------
durationMeasure
^^^^^^^^^^^^^^^

.. java:field:: protected DurationMeasure durationMeasure
   :outertype: NSGAIIMeasures

evaluations
^^^^^^^^^^^

.. java:field:: protected CountingMeasure evaluations
   :outertype: NSGAIIMeasures

hypervolumeValue
^^^^^^^^^^^^^^^^

.. java:field:: protected BasicMeasure<Double> hypervolumeValue
   :outertype: NSGAIIMeasures

measureManager
^^^^^^^^^^^^^^

.. java:field:: protected SimpleMeasureManager measureManager
   :outertype: NSGAIIMeasures

numberOfNonDominatedSolutionsInPopulation
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:field:: protected BasicMeasure<Integer> numberOfNonDominatedSolutionsInPopulation
   :outertype: NSGAIIMeasures

referenceFront
^^^^^^^^^^^^^^

.. java:field:: protected Front referenceFront
   :outertype: NSGAIIMeasures

solutionListMeasure
^^^^^^^^^^^^^^^^^^^

.. java:field:: protected BasicMeasure<List<S>> solutionListMeasure
   :outertype: NSGAIIMeasures

Constructors
------------
NSGAIIMeasures
^^^^^^^^^^^^^^

.. java:constructor:: public NSGAIIMeasures(Problem<S> problem, int maxIterations, int populationSize, CrossoverOperator<S> crossoverOperator, MutationOperator<S> mutationOperator, SelectionOperator<List<S>, S> selectionOperator, Comparator<S> dominanceComparator, SolutionListEvaluator<S> evaluator)
   :outertype: NSGAIIMeasures

   Constructor

Methods
-------
getDescription
^^^^^^^^^^^^^^

.. java:method:: @Override public String getDescription()
   :outertype: NSGAIIMeasures

getEvaluations
^^^^^^^^^^^^^^

.. java:method:: public CountingMeasure getEvaluations()
   :outertype: NSGAIIMeasures

getMeasureManager
^^^^^^^^^^^^^^^^^

.. java:method:: @Override public MeasureManager getMeasureManager()
   :outertype: NSGAIIMeasures

getName
^^^^^^^

.. java:method:: @Override public String getName()
   :outertype: NSGAIIMeasures

initProgress
^^^^^^^^^^^^

.. java:method:: @Override protected void initProgress()
   :outertype: NSGAIIMeasures

isStoppingConditionReached
^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override protected boolean isStoppingConditionReached()
   :outertype: NSGAIIMeasures

replacement
^^^^^^^^^^^

.. java:method:: @Override protected List<S> replacement(List<S> population, List<S> offspringPopulation)
   :outertype: NSGAIIMeasures

run
^^^

.. java:method:: @Override public void run()
   :outertype: NSGAIIMeasures

setReferenceFront
^^^^^^^^^^^^^^^^^

.. java:method:: public void setReferenceFront(Front referenceFront)
   :outertype: NSGAIIMeasures

updateProgress
^^^^^^^^^^^^^^

.. java:method:: @Override protected void updateProgress()
   :outertype: NSGAIIMeasures

