.. java:import:: org.uma.jmetal.operator MutationOperator

.. java:import:: org.uma.jmetal.operator.impl.mutation PolynomialMutation

.. java:import:: org.uma.jmetal.problem DoubleProblem

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.util AlgorithmBuilder

.. java:import:: org.uma.jmetal.util.archive BoundedArchive

.. java:import:: org.uma.jmetal.util.evaluator SolutionListEvaluator

.. java:import:: org.uma.jmetal.util.evaluator.impl SequentialSolutionListEvaluator

.. java:import:: org.uma.jmetal.util.pseudorandom JMetalRandom

.. java:import:: org.uma.jmetal.util.pseudorandom PseudoRandomGenerator

SMPSOBuilder
============

.. java:package:: org.uma.jmetal.algorithm.multiobjective.smpso
   :noindex:

.. java:type:: public class SMPSOBuilder implements AlgorithmBuilder<SMPSO>

   :author: Antonio J. Nebro

Fields
------
archiveSize
^^^^^^^^^^^

.. java:field:: protected int archiveSize
   :outertype: SMPSOBuilder

evaluator
^^^^^^^^^

.. java:field:: protected SolutionListEvaluator<DoubleSolution> evaluator
   :outertype: SMPSOBuilder

leaders
^^^^^^^

.. java:field:: protected BoundedArchive<DoubleSolution> leaders
   :outertype: SMPSOBuilder

mutationOperator
^^^^^^^^^^^^^^^^

.. java:field:: protected MutationOperator<DoubleSolution> mutationOperator
   :outertype: SMPSOBuilder

variant
^^^^^^^

.. java:field:: protected SMPSOVariant variant
   :outertype: SMPSOBuilder

Constructors
------------
SMPSOBuilder
^^^^^^^^^^^^

.. java:constructor:: public SMPSOBuilder(DoubleProblem problem, BoundedArchive<DoubleSolution> leaders)
   :outertype: SMPSOBuilder

Methods
-------
build
^^^^^

.. java:method:: public SMPSO build()
   :outertype: SMPSOBuilder

getArchiveSize
^^^^^^^^^^^^^^

.. java:method:: public int getArchiveSize()
   :outertype: SMPSOBuilder

getC1Max
^^^^^^^^

.. java:method:: public double getC1Max()
   :outertype: SMPSOBuilder

getC1Min
^^^^^^^^

.. java:method:: public double getC1Min()
   :outertype: SMPSOBuilder

getC2Max
^^^^^^^^

.. java:method:: public double getC2Max()
   :outertype: SMPSOBuilder

getC2Min
^^^^^^^^

.. java:method:: public double getC2Min()
   :outertype: SMPSOBuilder

getChangeVelocity1
^^^^^^^^^^^^^^^^^^

.. java:method:: public double getChangeVelocity1()
   :outertype: SMPSOBuilder

getChangeVelocity2
^^^^^^^^^^^^^^^^^^

.. java:method:: public double getChangeVelocity2()
   :outertype: SMPSOBuilder

getEvaluator
^^^^^^^^^^^^

.. java:method:: public SolutionListEvaluator<DoubleSolution> getEvaluator()
   :outertype: SMPSOBuilder

getLeaders
^^^^^^^^^^

.. java:method:: public BoundedArchive<DoubleSolution> getLeaders()
   :outertype: SMPSOBuilder

getMaxIterations
^^^^^^^^^^^^^^^^

.. java:method:: public int getMaxIterations()
   :outertype: SMPSOBuilder

getMutation
^^^^^^^^^^^

.. java:method:: public MutationOperator<DoubleSolution> getMutation()
   :outertype: SMPSOBuilder

getMutationOperator
^^^^^^^^^^^^^^^^^^^

.. java:method:: public MutationOperator<DoubleSolution> getMutationOperator()
   :outertype: SMPSOBuilder

getProblem
^^^^^^^^^^

.. java:method:: public DoubleProblem getProblem()
   :outertype: SMPSOBuilder

getR1Max
^^^^^^^^

.. java:method:: public double getR1Max()
   :outertype: SMPSOBuilder

getR1Min
^^^^^^^^

.. java:method:: public double getR1Min()
   :outertype: SMPSOBuilder

getR2Max
^^^^^^^^

.. java:method:: public double getR2Max()
   :outertype: SMPSOBuilder

getR2Min
^^^^^^^^

.. java:method:: public double getR2Min()
   :outertype: SMPSOBuilder

getSwarmSize
^^^^^^^^^^^^

.. java:method:: public int getSwarmSize()
   :outertype: SMPSOBuilder

getWeightMax
^^^^^^^^^^^^

.. java:method:: public double getWeightMax()
   :outertype: SMPSOBuilder

getWeightMin
^^^^^^^^^^^^

.. java:method:: public double getWeightMin()
   :outertype: SMPSOBuilder

setC1Max
^^^^^^^^

.. java:method:: public SMPSOBuilder setC1Max(double c1Max)
   :outertype: SMPSOBuilder

setC1Min
^^^^^^^^

.. java:method:: public SMPSOBuilder setC1Min(double c1Min)
   :outertype: SMPSOBuilder

setC2Max
^^^^^^^^

.. java:method:: public SMPSOBuilder setC2Max(double c2Max)
   :outertype: SMPSOBuilder

setC2Min
^^^^^^^^

.. java:method:: public SMPSOBuilder setC2Min(double c2Min)
   :outertype: SMPSOBuilder

setChangeVelocity1
^^^^^^^^^^^^^^^^^^

.. java:method:: public SMPSOBuilder setChangeVelocity1(double changeVelocity1)
   :outertype: SMPSOBuilder

setChangeVelocity2
^^^^^^^^^^^^^^^^^^

.. java:method:: public SMPSOBuilder setChangeVelocity2(double changeVelocity2)
   :outertype: SMPSOBuilder

setMaxIterations
^^^^^^^^^^^^^^^^

.. java:method:: public SMPSOBuilder setMaxIterations(int maxIterations)
   :outertype: SMPSOBuilder

setMutation
^^^^^^^^^^^

.. java:method:: public SMPSOBuilder setMutation(MutationOperator<DoubleSolution> mutation)
   :outertype: SMPSOBuilder

setR1Max
^^^^^^^^

.. java:method:: public SMPSOBuilder setR1Max(double r1Max)
   :outertype: SMPSOBuilder

setR1Min
^^^^^^^^

.. java:method:: public SMPSOBuilder setR1Min(double r1Min)
   :outertype: SMPSOBuilder

setR2Max
^^^^^^^^

.. java:method:: public SMPSOBuilder setR2Max(double r2Max)
   :outertype: SMPSOBuilder

setR2Min
^^^^^^^^

.. java:method:: public SMPSOBuilder setR2Min(double r2Min)
   :outertype: SMPSOBuilder

setRandomGenerator
^^^^^^^^^^^^^^^^^^

.. java:method:: public SMPSOBuilder setRandomGenerator(PseudoRandomGenerator randomGenerator)
   :outertype: SMPSOBuilder

setSolutionListEvaluator
^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public SMPSOBuilder setSolutionListEvaluator(SolutionListEvaluator<DoubleSolution> evaluator)
   :outertype: SMPSOBuilder

setSwarmSize
^^^^^^^^^^^^

.. java:method:: public SMPSOBuilder setSwarmSize(int swarmSize)
   :outertype: SMPSOBuilder

setVariant
^^^^^^^^^^

.. java:method:: public SMPSOBuilder setVariant(SMPSOVariant variant)
   :outertype: SMPSOBuilder

setWeightMax
^^^^^^^^^^^^

.. java:method:: public SMPSOBuilder setWeightMax(double weightMax)
   :outertype: SMPSOBuilder

setWeightMin
^^^^^^^^^^^^

.. java:method:: public SMPSOBuilder setWeightMin(double weightMin)
   :outertype: SMPSOBuilder

