.. java:import:: org.uma.jmetal.measure Measurable

.. java:import:: org.uma.jmetal.measure MeasureManager

.. java:import:: org.uma.jmetal.measure.impl BasicMeasure

.. java:import:: org.uma.jmetal.measure.impl CountingMeasure

.. java:import:: org.uma.jmetal.measure.impl DurationMeasure

.. java:import:: org.uma.jmetal.measure.impl SimpleMeasureManager

.. java:import:: org.uma.jmetal.problem DoubleProblem

.. java:import:: org.uma.jmetal.qualityindicator.impl Epsilon

.. java:import:: org.uma.jmetal.qualityindicator.impl.hypervolume PISAHypervolume

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.util.front Front

.. java:import:: org.uma.jmetal.util.front.imp ArrayFront

.. java:import:: java.util List

DMOPSOMeasures
==============

.. java:package:: org.uma.jmetal.algorithm.multiobjective.dmopso
   :noindex:

.. java:type:: @SuppressWarnings public class DMOPSOMeasures extends DMOPSO implements Measurable

Fields
------
durationMeasure
^^^^^^^^^^^^^^^

.. java:field:: protected DurationMeasure durationMeasure
   :outertype: DMOPSOMeasures

epsilonValue
^^^^^^^^^^^^

.. java:field:: protected BasicMeasure<Double> epsilonValue
   :outertype: DMOPSOMeasures

hypervolumeValue
^^^^^^^^^^^^^^^^

.. java:field:: protected BasicMeasure<Double> hypervolumeValue
   :outertype: DMOPSOMeasures

iterations
^^^^^^^^^^

.. java:field:: protected CountingMeasure iterations
   :outertype: DMOPSOMeasures

measureManager
^^^^^^^^^^^^^^

.. java:field:: protected SimpleMeasureManager measureManager
   :outertype: DMOPSOMeasures

referenceFront
^^^^^^^^^^^^^^

.. java:field:: protected Front referenceFront
   :outertype: DMOPSOMeasures

solutionListMeasure
^^^^^^^^^^^^^^^^^^^

.. java:field:: protected BasicMeasure<List<DoubleSolution>> solutionListMeasure
   :outertype: DMOPSOMeasures

Constructors
------------
DMOPSOMeasures
^^^^^^^^^^^^^^

.. java:constructor:: public DMOPSOMeasures(DoubleProblem problem, int swarmSize, int maxIterations, double r1Min, double r1Max, double r2Min, double r2Max, double c1Min, double c1Max, double c2Min, double c2Max, double weightMin, double weightMax, double changeVelocity1, double changeVelocity2, FunctionType functionType, String dataDirectory, int maxAge)
   :outertype: DMOPSOMeasures

DMOPSOMeasures
^^^^^^^^^^^^^^

.. java:constructor:: public DMOPSOMeasures(DoubleProblem problem, int swarmSize, int maxIterations, double r1Min, double r1Max, double r2Min, double r2Max, double c1Min, double c1Max, double c2Min, double c2Max, double weightMin, double weightMax, double changeVelocity1, double changeVelocity2, FunctionType functionType, String dataDirectory, int maxAge, String name)
   :outertype: DMOPSOMeasures

Methods
-------
getDescription
^^^^^^^^^^^^^^

.. java:method:: @Override public String getDescription()
   :outertype: DMOPSOMeasures

getMeasureManager
^^^^^^^^^^^^^^^^^

.. java:method:: @Override public MeasureManager getMeasureManager()
   :outertype: DMOPSOMeasures

initProgress
^^^^^^^^^^^^

.. java:method:: @Override protected void initProgress()
   :outertype: DMOPSOMeasures

isStoppingConditionReached
^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override protected boolean isStoppingConditionReached()
   :outertype: DMOPSOMeasures

run
^^^

.. java:method:: @Override public void run()
   :outertype: DMOPSOMeasures

setReferenceFront
^^^^^^^^^^^^^^^^^

.. java:method:: public void setReferenceFront(Front referenceFront)
   :outertype: DMOPSOMeasures

updateProgress
^^^^^^^^^^^^^^

.. java:method:: @Override protected void updateProgress()
   :outertype: DMOPSOMeasures

