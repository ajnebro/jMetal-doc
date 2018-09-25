.. java:import:: org.uma.jmetal.algorithm.impl AbstractParticleSwarmOptimization

.. java:import:: org.uma.jmetal.operator MutationOperator

.. java:import:: org.uma.jmetal.problem DoubleProblem

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.util.archive BoundedArchive

.. java:import:: org.uma.jmetal.util.comparator DominanceComparator

.. java:import:: org.uma.jmetal.util.evaluator SolutionListEvaluator

.. java:import:: org.uma.jmetal.util.pseudorandom JMetalRandom

.. java:import:: org.uma.jmetal.util.solutionattribute.impl GenericSolutionAttribute

.. java:import:: java.util ArrayList

.. java:import:: java.util Comparator

.. java:import:: java.util List

SMPSO
=====

.. java:package:: org.uma.jmetal.algorithm.multiobjective.smpso
   :noindex:

.. java:type:: @SuppressWarnings public class SMPSO extends AbstractParticleSwarmOptimization<DoubleSolution, List<DoubleSolution>>

   This class implements the SMPSO algorithm described in: SMPSO: A new PSO-based metaheuristic for multi-objective optimization MCDM 2009. DOI: http://dx.doi.org/10.1109/MCDM.2009.4938830

   :author: Antonio J. Nebro

Constructors
------------
SMPSO
^^^^^

.. java:constructor:: public SMPSO(DoubleProblem problem, int swarmSize, BoundedArchive<DoubleSolution> leaders, MutationOperator<DoubleSolution> mutationOperator, int maxIterations, double r1Min, double r1Max, double r2Min, double r2Max, double c1Min, double c1Max, double c2Min, double c2Max, double weightMin, double weightMax, double changeVelocity1, double changeVelocity2, SolutionListEvaluator<DoubleSolution> evaluator)
   :outertype: SMPSO

   Constructor

Methods
-------
constrictionCoefficient
^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: protected double constrictionCoefficient(double c1, double c2)
   :outertype: SMPSO

createInitialSwarm
^^^^^^^^^^^^^^^^^^

.. java:method:: @Override protected List<DoubleSolution> createInitialSwarm()
   :outertype: SMPSO

evaluateSwarm
^^^^^^^^^^^^^

.. java:method:: @Override protected List<DoubleSolution> evaluateSwarm(List<DoubleSolution> swarm)
   :outertype: SMPSO

getDescription
^^^^^^^^^^^^^^

.. java:method:: @Override public String getDescription()
   :outertype: SMPSO

getIterations
^^^^^^^^^^^^^

.. java:method:: public int getIterations()
   :outertype: SMPSO

getMaxIterations
^^^^^^^^^^^^^^^^

.. java:method:: public int getMaxIterations()
   :outertype: SMPSO

getName
^^^^^^^

.. java:method:: @Override public String getName()
   :outertype: SMPSO

getResult
^^^^^^^^^

.. java:method:: @Override public List<DoubleSolution> getResult()
   :outertype: SMPSO

getSwarmSize
^^^^^^^^^^^^

.. java:method:: public int getSwarmSize()
   :outertype: SMPSO

initProgress
^^^^^^^^^^^^

.. java:method:: @Override protected void initProgress()
   :outertype: SMPSO

initializeLeader
^^^^^^^^^^^^^^^^

.. java:method:: @Override protected void initializeLeader(List<DoubleSolution> swarm)
   :outertype: SMPSO

initializeParticlesMemory
^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override protected void initializeParticlesMemory(List<DoubleSolution> swarm)
   :outertype: SMPSO

initializeVelocity
^^^^^^^^^^^^^^^^^^

.. java:method:: @Override protected void initializeVelocity(List<DoubleSolution> swarm)
   :outertype: SMPSO

isStoppingConditionReached
^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override protected boolean isStoppingConditionReached()
   :outertype: SMPSO

perturbation
^^^^^^^^^^^^

.. java:method:: @Override protected void perturbation(List<DoubleSolution> swarm)
   :outertype: SMPSO

selectGlobalBest
^^^^^^^^^^^^^^^^

.. java:method:: protected DoubleSolution selectGlobalBest()
   :outertype: SMPSO

setIterations
^^^^^^^^^^^^^

.. java:method:: public void setIterations(int iterations)
   :outertype: SMPSO

updateLeaders
^^^^^^^^^^^^^

.. java:method:: @Override protected void updateLeaders(List<DoubleSolution> swarm)
   :outertype: SMPSO

updateLeadersDensityEstimator
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: protected void updateLeadersDensityEstimator()
   :outertype: SMPSO

updateParticlesMemory
^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override protected void updateParticlesMemory(List<DoubleSolution> swarm)
   :outertype: SMPSO

updatePosition
^^^^^^^^^^^^^^

.. java:method:: @Override protected void updatePosition(List<DoubleSolution> swarm)
   :outertype: SMPSO

updateProgress
^^^^^^^^^^^^^^

.. java:method:: @Override protected void updateProgress()
   :outertype: SMPSO

updateVelocity
^^^^^^^^^^^^^^

.. java:method:: @Override protected void updateVelocity(List<DoubleSolution> swarm)
   :outertype: SMPSO

