.. java:import:: org.uma.jmetal.algorithm.impl AbstractParticleSwarmOptimization

.. java:import:: org.uma.jmetal.operator.impl.mutation NonUniformMutation

.. java:import:: org.uma.jmetal.operator.impl.mutation UniformMutation

.. java:import:: org.uma.jmetal.problem DoubleProblem

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.util.archive.impl CrowdingDistanceArchive

.. java:import:: org.uma.jmetal.util.archive.impl NonDominatedSolutionListArchive

.. java:import:: org.uma.jmetal.util.comparator CrowdingDistanceComparator

.. java:import:: org.uma.jmetal.util.comparator DominanceComparator

.. java:import:: org.uma.jmetal.util.evaluator SolutionListEvaluator

.. java:import:: org.uma.jmetal.util.pseudorandom JMetalRandom

.. java:import:: org.uma.jmetal.util.solutionattribute.impl CrowdingDistance

.. java:import:: java.util ArrayList

.. java:import:: java.util Comparator

.. java:import:: java.util List

OMOPSO
======

.. java:package:: org.uma.jmetal.algorithm.multiobjective.omopso
   :noindex:

.. java:type:: @SuppressWarnings public class OMOPSO extends AbstractParticleSwarmOptimization<DoubleSolution, List<DoubleSolution>>

   Class implementing the OMOPSO algorithm

Fields
------
evaluator
^^^^^^^^^

.. java:field::  SolutionListEvaluator<DoubleSolution> evaluator
   :outertype: OMOPSO

Constructors
------------
OMOPSO
^^^^^^

.. java:constructor:: public OMOPSO(DoubleProblem problem, SolutionListEvaluator<DoubleSolution> evaluator, int swarmSize, int maxIterations, int archiveSize, UniformMutation uniformMutation, NonUniformMutation nonUniformMutation)
   :outertype: OMOPSO

   Constructor

Methods
-------
createInitialSwarm
^^^^^^^^^^^^^^^^^^

.. java:method:: @Override protected List<DoubleSolution> createInitialSwarm()
   :outertype: OMOPSO

evaluateSwarm
^^^^^^^^^^^^^

.. java:method:: @Override protected List<DoubleSolution> evaluateSwarm(List<DoubleSolution> swarm)
   :outertype: OMOPSO

getDescription
^^^^^^^^^^^^^^

.. java:method:: @Override public String getDescription()
   :outertype: OMOPSO

getName
^^^^^^^

.. java:method:: @Override public String getName()
   :outertype: OMOPSO

getResult
^^^^^^^^^

.. java:method:: @Override public List<DoubleSolution> getResult()
   :outertype: OMOPSO

initProgress
^^^^^^^^^^^^

.. java:method:: @Override protected void initProgress()
   :outertype: OMOPSO

initializeLeader
^^^^^^^^^^^^^^^^

.. java:method:: @Override protected void initializeLeader(List<DoubleSolution> swarm)
   :outertype: OMOPSO

initializeParticlesMemory
^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override protected void initializeParticlesMemory(List<DoubleSolution> swarm)
   :outertype: OMOPSO

initializeVelocity
^^^^^^^^^^^^^^^^^^

.. java:method:: @Override protected void initializeVelocity(List<DoubleSolution> swarm)
   :outertype: OMOPSO

isStoppingConditionReached
^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override protected boolean isStoppingConditionReached()
   :outertype: OMOPSO

perturbation
^^^^^^^^^^^^

.. java:method:: @Override protected void perturbation(List<DoubleSolution> swarm)
   :outertype: OMOPSO

   Apply a mutation operator to all particles in the swarm (perturbation)

tearDown
^^^^^^^^

.. java:method:: protected void tearDown()
   :outertype: OMOPSO

updateLeaders
^^^^^^^^^^^^^

.. java:method:: @Override protected void updateLeaders(List<DoubleSolution> swarm)
   :outertype: OMOPSO

   Update leaders method

   :param swarm: List of solutions (swarm)

updateParticlesMemory
^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override protected void updateParticlesMemory(List<DoubleSolution> swarm)
   :outertype: OMOPSO

updatePosition
^^^^^^^^^^^^^^

.. java:method:: @Override protected void updatePosition(List<DoubleSolution> swarm)
   :outertype: OMOPSO

   Update the position of each particle

updateProgress
^^^^^^^^^^^^^^

.. java:method:: @Override protected void updateProgress()
   :outertype: OMOPSO

updateVelocity
^^^^^^^^^^^^^^

.. java:method:: @Override protected void updateVelocity(List<DoubleSolution> swarm)
   :outertype: OMOPSO

