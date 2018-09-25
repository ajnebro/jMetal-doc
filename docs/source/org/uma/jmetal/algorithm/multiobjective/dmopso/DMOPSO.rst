.. java:import:: org.uma.jmetal.algorithm Algorithm

.. java:import:: org.uma.jmetal.problem DoubleProblem

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: org.uma.jmetal.util.evaluator SolutionListEvaluator

.. java:import:: org.uma.jmetal.util.evaluator.impl SequentialSolutionListEvaluator

.. java:import:: org.uma.jmetal.util.pseudorandom JMetalRandom

.. java:import:: java.io BufferedReader

.. java:import:: java.io InputStream

.. java:import:: java.io InputStreamReader

.. java:import:: java.util ArrayList

.. java:import:: java.util Arrays

.. java:import:: java.util List

.. java:import:: java.util StringTokenizer

DMOPSO
======

.. java:package:: org.uma.jmetal.algorithm.multiobjective.dmopso
   :noindex:

.. java:type:: @SuppressWarnings public class DMOPSO implements Algorithm<List<DoubleSolution>>

Fields
------
dataDirectory
^^^^^^^^^^^^^

.. java:field::  String dataDirectory
   :outertype: DMOPSO

functionType
^^^^^^^^^^^^

.. java:field::  FunctionType functionType
   :outertype: DMOPSO

indArray
^^^^^^^^

.. java:field::  DoubleSolution[] indArray
   :outertype: DMOPSO

iterations
^^^^^^^^^^

.. java:field:: protected int iterations
   :outertype: DMOPSO

lambda
^^^^^^

.. java:field::  double[][] lambda
   :outertype: DMOPSO

maxAge
^^^^^^

.. java:field:: protected int maxAge
   :outertype: DMOPSO

maxIterations
^^^^^^^^^^^^^

.. java:field:: protected int maxIterations
   :outertype: DMOPSO

swarmSize
^^^^^^^^^

.. java:field:: protected int swarmSize
   :outertype: DMOPSO

z
^

.. java:field::  double[] z
   :outertype: DMOPSO

Constructors
------------
DMOPSO
^^^^^^

.. java:constructor:: public DMOPSO(DoubleProblem problem, int swarmSize, int maxIterations, double r1Min, double r1Max, double r2Min, double r2Max, double c1Min, double c1Max, double c2Min, double c2Max, double weightMin, double weightMax, double changeVelocity1, double changeVelocity2, FunctionType functionType, String dataDirectory, int maxAge)
   :outertype: DMOPSO

DMOPSO
^^^^^^

.. java:constructor:: public DMOPSO(DoubleProblem problem, int swarmSize, int maxIterations, double r1Min, double r1Max, double r2Min, double r2Max, double c1Min, double c1Max, double c2Min, double c2Max, double weightMin, double weightMax, double changeVelocity1, double changeVelocity2, FunctionType functionType, String dataDirectory, int maxAge, String name)
   :outertype: DMOPSO

Methods
-------
createInitialSwarm
^^^^^^^^^^^^^^^^^^

.. java:method:: protected List<DoubleSolution> createInitialSwarm()
   :outertype: DMOPSO

evaluateSwarm
^^^^^^^^^^^^^

.. java:method:: protected List<DoubleSolution> evaluateSwarm(List<DoubleSolution> swarm)
   :outertype: DMOPSO

getDescription
^^^^^^^^^^^^^^

.. java:method:: @Override public String getDescription()
   :outertype: DMOPSO

getName
^^^^^^^

.. java:method:: @Override public String getName()
   :outertype: DMOPSO

getResult
^^^^^^^^^

.. java:method:: @Override public List<DoubleSolution> getResult()
   :outertype: DMOPSO

getSwarm
^^^^^^^^

.. java:method:: public List<DoubleSolution> getSwarm()
   :outertype: DMOPSO

initProgress
^^^^^^^^^^^^

.. java:method:: protected void initProgress()
   :outertype: DMOPSO

initializeLeaders
^^^^^^^^^^^^^^^^^

.. java:method:: protected void initializeLeaders(List<DoubleSolution> swarm)
   :outertype: DMOPSO

initializeParticlesMemory
^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: protected void initializeParticlesMemory(List<DoubleSolution> swarm)
   :outertype: DMOPSO

initializeVelocity
^^^^^^^^^^^^^^^^^^

.. java:method:: protected void initializeVelocity(List<DoubleSolution> swarm)
   :outertype: DMOPSO

isStoppingConditionReached
^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: protected boolean isStoppingConditionReached()
   :outertype: DMOPSO

run
^^^

.. java:method:: @Override public void run()
   :outertype: DMOPSO

updateProgress
^^^^^^^^^^^^^^

.. java:method:: protected void updateProgress()
   :outertype: DMOPSO

updateVelocity
^^^^^^^^^^^^^^

.. java:method:: protected void updateVelocity(int i)
   :outertype: DMOPSO

