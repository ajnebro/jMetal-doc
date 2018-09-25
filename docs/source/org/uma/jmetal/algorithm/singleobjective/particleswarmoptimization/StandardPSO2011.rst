.. java:import:: org.uma.jmetal.algorithm.impl AbstractParticleSwarmOptimization

.. java:import:: org.uma.jmetal.operator Operator

.. java:import:: org.uma.jmetal.operator.impl.selection BestSolutionSelection

.. java:import:: org.uma.jmetal.problem DoubleProblem

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.util SolutionUtils

.. java:import:: org.uma.jmetal.util.comparator ObjectiveComparator

.. java:import:: org.uma.jmetal.util.evaluator SolutionListEvaluator

.. java:import:: org.uma.jmetal.util.neighborhood.impl AdaptiveRandomNeighborhood

.. java:import:: org.uma.jmetal.util.pseudorandom JMetalRandom

.. java:import:: org.uma.jmetal.util.pseudorandom.impl ExtendedPseudoRandomGenerator

.. java:import:: org.uma.jmetal.util.pseudorandom.impl JavaRandomGenerator

.. java:import:: org.uma.jmetal.util.solutionattribute.impl GenericSolutionAttribute

.. java:import:: java.util ArrayList

.. java:import:: java.util Comparator

.. java:import:: java.util List

StandardPSO2011
===============

.. java:package:: org.uma.jmetal.algorithm.singleobjective.particleswarmoptimization
   :noindex:

.. java:type:: @SuppressWarnings public class StandardPSO2011 extends AbstractParticleSwarmOptimization<DoubleSolution, DoubleSolution>

   Class implementing a Standard PSO 2011 algorithm.

   :author: Antonio J. Nebro

Constructors
------------
StandardPSO2011
^^^^^^^^^^^^^^^

.. java:constructor:: public StandardPSO2011(DoubleProblem problem, int objectiveId, int swarmSize, int maxIterations, int numberOfParticlesToInform, SolutionListEvaluator<DoubleSolution> evaluator)
   :outertype: StandardPSO2011

   Constructor

   :param problem:
   :param objectiveId: This field indicates which objective, in the case of a multi-objective problem, is selected to be optimized.
   :param swarmSize:
   :param maxIterations:
   :param numberOfParticlesToInform:
   :param evaluator:

StandardPSO2011
^^^^^^^^^^^^^^^

.. java:constructor:: public StandardPSO2011(DoubleProblem problem, int swarmSize, int maxIterations, int numberOfParticlesToInform, SolutionListEvaluator<DoubleSolution> evaluator)
   :outertype: StandardPSO2011

   Constructor

   :param problem:
   :param swarmSize:
   :param maxIterations:
   :param numberOfParticlesToInform:
   :param evaluator:

Methods
-------
createInitialSwarm
^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public List<DoubleSolution> createInitialSwarm()
   :outertype: StandardPSO2011

evaluateSwarm
^^^^^^^^^^^^^

.. java:method:: @Override public List<DoubleSolution> evaluateSwarm(List<DoubleSolution> swarm)
   :outertype: StandardPSO2011

getDescription
^^^^^^^^^^^^^^

.. java:method:: @Override public String getDescription()
   :outertype: StandardPSO2011

getLocalBest
^^^^^^^^^^^^

.. java:method:: public DoubleSolution[] getLocalBest()
   :outertype: StandardPSO2011

getName
^^^^^^^

.. java:method:: @Override public String getName()
   :outertype: StandardPSO2011

getResult
^^^^^^^^^

.. java:method:: @Override public DoubleSolution getResult()
   :outertype: StandardPSO2011

getSwarmSpeedMatrix
^^^^^^^^^^^^^^^^^^^

.. java:method:: public double[][] getSwarmSpeedMatrix()
   :outertype: StandardPSO2011

initProgress
^^^^^^^^^^^^

.. java:method:: @Override public void initProgress()
   :outertype: StandardPSO2011

initializeLeader
^^^^^^^^^^^^^^^^

.. java:method:: @Override public void initializeLeader(List<DoubleSolution> swarm)
   :outertype: StandardPSO2011

initializeParticlesMemory
^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public void initializeParticlesMemory(List<DoubleSolution> swarm)
   :outertype: StandardPSO2011

initializeVelocity
^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public void initializeVelocity(List<DoubleSolution> swarm)
   :outertype: StandardPSO2011

isStoppingConditionReached
^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public boolean isStoppingConditionReached()
   :outertype: StandardPSO2011

perturbation
^^^^^^^^^^^^

.. java:method:: @Override public void perturbation(List<DoubleSolution> swarm)
   :outertype: StandardPSO2011

updateLeaders
^^^^^^^^^^^^^

.. java:method:: @Override public void updateLeaders(List<DoubleSolution> swarm)
   :outertype: StandardPSO2011

updateParticlesMemory
^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public void updateParticlesMemory(List<DoubleSolution> swarm)
   :outertype: StandardPSO2011

updatePosition
^^^^^^^^^^^^^^

.. java:method:: @Override public void updatePosition(List<DoubleSolution> swarm)
   :outertype: StandardPSO2011

updateProgress
^^^^^^^^^^^^^^

.. java:method:: @Override public void updateProgress()
   :outertype: StandardPSO2011

updateVelocity
^^^^^^^^^^^^^^

.. java:method:: @Override public void updateVelocity(List<DoubleSolution> swarm)
   :outertype: StandardPSO2011

