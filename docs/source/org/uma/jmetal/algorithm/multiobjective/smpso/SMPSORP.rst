.. java:import:: org.uma.jmetal.algorithm.impl AbstractParticleSwarmOptimization

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

.. java:import:: org.uma.jmetal.util.archivewithreferencepoint ArchiveWithReferencePoint

.. java:import:: org.uma.jmetal.util.comparator DominanceComparator

.. java:import:: org.uma.jmetal.util.evaluator SolutionListEvaluator

.. java:import:: org.uma.jmetal.util.pseudorandom JMetalRandom

.. java:import:: org.uma.jmetal.util.solutionattribute.impl GenericSolutionAttribute

.. java:import:: java.util ArrayList

.. java:import:: java.util Comparator

.. java:import:: java.util List

SMPSORP
=======

.. java:package:: org.uma.jmetal.algorithm.multiobjective.smpso
   :noindex:

.. java:type:: public class SMPSORP extends AbstractParticleSwarmOptimization<DoubleSolution, List<DoubleSolution>> implements Measurable

   This class implements the SMPSORP algorithm described in: "Extending the Speed-constrained Multi-Objective PSO (SMPSO) With Reference Point Based Preference Articulation. Antonio J. Nebro, Juan J. Durillo, José García-Nieto, Cristóbal Barba-González, Javier Del Ser, Carlos A. Coello Coello, Antonio Benítez-Hidalgo, José F. Aldana-Montes. Parallel Problem Solving from Nature -- PPSN XV. Lecture Notes In Computer Science, Vol. 11101, pp. 298-310. 2018".

   :author: Antonio J. Nebro

Fields
------
currentIteration
^^^^^^^^^^^^^^^^

.. java:field:: protected CountingMeasure currentIteration
   :outertype: SMPSORP

deltaMax
^^^^^^^^

.. java:field:: protected double deltaMax
   :outertype: SMPSORP

deltaMin
^^^^^^^^

.. java:field:: protected double deltaMin
   :outertype: SMPSORP

durationMeasure
^^^^^^^^^^^^^^^

.. java:field:: protected DurationMeasure durationMeasure
   :outertype: SMPSORP

evaluator
^^^^^^^^^

.. java:field:: protected SolutionListEvaluator<DoubleSolution> evaluator
   :outertype: SMPSORP

iterations
^^^^^^^^^^

.. java:field:: protected int iterations
   :outertype: SMPSORP

leaders
^^^^^^^

.. java:field:: public List<ArchiveWithReferencePoint<DoubleSolution>> leaders
   :outertype: SMPSORP

maxIterations
^^^^^^^^^^^^^

.. java:field:: protected int maxIterations
   :outertype: SMPSORP

measureManager
^^^^^^^^^^^^^^

.. java:field:: protected SimpleMeasureManager measureManager
   :outertype: SMPSORP

referencePoints
^^^^^^^^^^^^^^^

.. java:field:: protected List<List<Double>> referencePoints
   :outertype: SMPSORP

solutionListMeasure
^^^^^^^^^^^^^^^^^^^

.. java:field:: protected BasicMeasure<List<DoubleSolution>> solutionListMeasure
   :outertype: SMPSORP

swarmSize
^^^^^^^^^

.. java:field:: protected int swarmSize
   :outertype: SMPSORP

Constructors
------------
SMPSORP
^^^^^^^

.. java:constructor:: public SMPSORP(DoubleProblem problem, int swarmSize, List<ArchiveWithReferencePoint<DoubleSolution>> leaders, List<List<Double>> referencePoints, MutationOperator<DoubleSolution> mutationOperator, int maxIterations, double r1Min, double r1Max, double r2Min, double r2Max, double c1Min, double c1Max, double c2Min, double c2Max, double weightMin, double weightMax, double changeVelocity1, double changeVelocity2, SolutionListEvaluator<DoubleSolution> evaluator)
   :outertype: SMPSORP

   Constructor

Methods
-------
changeReferencePoints
^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public synchronized void changeReferencePoints(List<List<Double>> referencePoints)
   :outertype: SMPSORP

createInitialSwarm
^^^^^^^^^^^^^^^^^^

.. java:method:: @Override protected List<DoubleSolution> createInitialSwarm()
   :outertype: SMPSORP

evaluateSwarm
^^^^^^^^^^^^^

.. java:method:: @Override protected List<DoubleSolution> evaluateSwarm(List<DoubleSolution> swarm)
   :outertype: SMPSORP

getDescription
^^^^^^^^^^^^^^

.. java:method:: @Override public String getDescription()
   :outertype: SMPSORP

getMeasureManager
^^^^^^^^^^^^^^^^^

.. java:method:: @Override public MeasureManager getMeasureManager()
   :outertype: SMPSORP

getName
^^^^^^^

.. java:method:: @Override public String getName()
   :outertype: SMPSORP

getResult
^^^^^^^^^

.. java:method:: @Override public List<DoubleSolution> getResult()
   :outertype: SMPSORP

initProgress
^^^^^^^^^^^^

.. java:method:: @Override protected void initProgress()
   :outertype: SMPSORP

initializeLeader
^^^^^^^^^^^^^^^^

.. java:method:: @Override protected void initializeLeader(List<DoubleSolution> swarm)
   :outertype: SMPSORP

initializeParticlesMemory
^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override protected void initializeParticlesMemory(List<DoubleSolution> swarm)
   :outertype: SMPSORP

initializeVelocity
^^^^^^^^^^^^^^^^^^

.. java:method:: @Override protected void initializeVelocity(List<DoubleSolution> swarm)
   :outertype: SMPSORP

isStoppingConditionReached
^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override protected boolean isStoppingConditionReached()
   :outertype: SMPSORP

perturbation
^^^^^^^^^^^^

.. java:method:: @Override protected void perturbation(List<DoubleSolution> swarm)
   :outertype: SMPSORP

removeDominatedSolutionsInArchives
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public void removeDominatedSolutionsInArchives()
   :outertype: SMPSORP

selectGlobalBest
^^^^^^^^^^^^^^^^

.. java:method:: protected DoubleSolution selectGlobalBest()
   :outertype: SMPSORP

updateLeaders
^^^^^^^^^^^^^

.. java:method:: @Override protected void updateLeaders(List<DoubleSolution> swarm)
   :outertype: SMPSORP

updateLeadersDensityEstimator
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: protected void updateLeadersDensityEstimator()
   :outertype: SMPSORP

updateParticlesMemory
^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override protected void updateParticlesMemory(List<DoubleSolution> swarm)
   :outertype: SMPSORP

updatePosition
^^^^^^^^^^^^^^

.. java:method:: @Override protected void updatePosition(List<DoubleSolution> swarm)
   :outertype: SMPSORP

updateProgress
^^^^^^^^^^^^^^

.. java:method:: @Override protected void updateProgress()
   :outertype: SMPSORP

updateVelocity
^^^^^^^^^^^^^^

.. java:method:: @Override protected void updateVelocity(List<DoubleSolution> swarm)
   :outertype: SMPSORP

