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

.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util.evaluator SolutionListEvaluator

.. java:import:: java.util List

WASFGAMeasures
==============

.. java:package:: org.uma.jmetal.algorithm.multiobjective.wasfga
   :noindex:

.. java:type:: @SuppressWarnings public class WASFGAMeasures<S extends Solution<?>> extends WASFGA<S> implements Measurable

   Implementation of the preference based algorithm named WASF-GA on jMetal5.0

   :author: Jorge Rodriguez

Fields
------
durationMeasure
^^^^^^^^^^^^^^^

.. java:field:: protected DurationMeasure durationMeasure
   :outertype: WASFGAMeasures

iterations
^^^^^^^^^^

.. java:field:: protected CountingMeasure iterations
   :outertype: WASFGAMeasures

measureManager
^^^^^^^^^^^^^^

.. java:field:: protected SimpleMeasureManager measureManager
   :outertype: WASFGAMeasures

solutionListMeasure
^^^^^^^^^^^^^^^^^^^

.. java:field:: protected BasicMeasure<List<S>> solutionListMeasure
   :outertype: WASFGAMeasures

Constructors
------------
WASFGAMeasures
^^^^^^^^^^^^^^

.. java:constructor:: public WASFGAMeasures(Problem<S> problem, int populationSize, int maxIterations, CrossoverOperator<S> crossoverOperator, MutationOperator<S> mutationOperator, SelectionOperator<List<S>, S> selectionOperator, SolutionListEvaluator<S> evaluator, double epsilon, List<Double> referencePoint, String weightVectorsFileName)
   :outertype: WASFGAMeasures

   Constructor

   :param problem: Problem to solve

WASFGAMeasures
^^^^^^^^^^^^^^

.. java:constructor:: public WASFGAMeasures(Problem<S> problem, int populationSize, int maxIterations, CrossoverOperator<S> crossoverOperator, MutationOperator<S> mutationOperator, SelectionOperator<List<S>, S> selectionOperator, SolutionListEvaluator<S> evaluator, double epsilon, List<Double> referencePoint)
   :outertype: WASFGAMeasures

   Constructor

   :param problem: Problem to solve

Methods
-------
getDescription
^^^^^^^^^^^^^^

.. java:method:: @Override public String getDescription()
   :outertype: WASFGAMeasures

getMeasureManager
^^^^^^^^^^^^^^^^^

.. java:method:: @Override public MeasureManager getMeasureManager()
   :outertype: WASFGAMeasures

getName
^^^^^^^

.. java:method:: @Override public String getName()
   :outertype: WASFGAMeasures

initProgress
^^^^^^^^^^^^

.. java:method:: @Override protected void initProgress()
   :outertype: WASFGAMeasures

isStoppingConditionReached
^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override protected boolean isStoppingConditionReached()
   :outertype: WASFGAMeasures

run
^^^

.. java:method:: @Override public void run()
   :outertype: WASFGAMeasures

updateProgress
^^^^^^^^^^^^^^

.. java:method:: @Override protected void updateProgress()
   :outertype: WASFGAMeasures

