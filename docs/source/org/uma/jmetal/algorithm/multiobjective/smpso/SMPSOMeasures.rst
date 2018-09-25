.. java:import:: org.uma.jmetal.measure Measurable

.. java:import:: org.uma.jmetal.measure MeasureManager

.. java:import:: org.uma.jmetal.measure.impl BasicMeasure

.. java:import:: org.uma.jmetal.measure.impl CountingMeasure

.. java:import:: org.uma.jmetal.measure.impl DurationMeasure

.. java:import:: org.uma.jmetal.measure.impl SimpleMeasureManager

.. java:import:: org.uma.jmetal.operator MutationOperator

.. java:import:: org.uma.jmetal.problem DoubleProblem

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.util.archive BoundedArchive

.. java:import:: org.uma.jmetal.util.evaluator SolutionListEvaluator

.. java:import:: java.util List

SMPSOMeasures
=============

.. java:package:: org.uma.jmetal.algorithm.multiobjective.smpso
   :noindex:

.. java:type:: @SuppressWarnings public class SMPSOMeasures extends SMPSO implements Measurable

   This class implements a version of SMPSO using measures

   :author: Antonio J. Nebro

Fields
------
durationMeasure
^^^^^^^^^^^^^^^

.. java:field:: protected DurationMeasure durationMeasure
   :outertype: SMPSOMeasures

iterations
^^^^^^^^^^

.. java:field:: protected CountingMeasure iterations
   :outertype: SMPSOMeasures

measureManager
^^^^^^^^^^^^^^

.. java:field:: protected SimpleMeasureManager measureManager
   :outertype: SMPSOMeasures

solutionListMeasure
^^^^^^^^^^^^^^^^^^^

.. java:field:: protected BasicMeasure<List<DoubleSolution>> solutionListMeasure
   :outertype: SMPSOMeasures

Constructors
------------
SMPSOMeasures
^^^^^^^^^^^^^

.. java:constructor:: public SMPSOMeasures(DoubleProblem problem, int swarmSize, BoundedArchive<DoubleSolution> leaders, MutationOperator<DoubleSolution> mutationOperator, int maxIterations, double r1Min, double r1Max, double r2Min, double r2Max, double c1Min, double c1Max, double c2Min, double c2Max, double weightMin, double weightMax, double changeVelocity1, double changeVelocity2, SolutionListEvaluator<DoubleSolution> evaluator)
   :outertype: SMPSOMeasures

   Constructor

   :param problem:
   :param swarmSize:
   :param leaders:
   :param mutationOperator:
   :param maxIterations:
   :param r1Min:
   :param r1Max:
   :param r2Min:
   :param r2Max:
   :param c1Min:
   :param c1Max:
   :param c2Min:
   :param c2Max:
   :param weightMin:
   :param weightMax:
   :param changeVelocity1:
   :param changeVelocity2:
   :param evaluator:

Methods
-------
getDescription
^^^^^^^^^^^^^^

.. java:method:: @Override public String getDescription()
   :outertype: SMPSOMeasures

getMeasureManager
^^^^^^^^^^^^^^^^^

.. java:method:: @Override public MeasureManager getMeasureManager()
   :outertype: SMPSOMeasures

getName
^^^^^^^

.. java:method:: @Override public String getName()
   :outertype: SMPSOMeasures

initProgress
^^^^^^^^^^^^

.. java:method:: @Override protected void initProgress()
   :outertype: SMPSOMeasures

isStoppingConditionReached
^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override protected boolean isStoppingConditionReached()
   :outertype: SMPSOMeasures

run
^^^

.. java:method:: @Override public void run()
   :outertype: SMPSOMeasures

updateProgress
^^^^^^^^^^^^^^

.. java:method:: @Override protected void updateProgress()
   :outertype: SMPSOMeasures

