.. java:import:: org.uma.jmetal.problem DoubleProblem

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.util AlgorithmBuilder

.. java:import:: org.uma.jmetal.util.evaluator SolutionListEvaluator

.. java:import:: org.uma.jmetal.util.evaluator.impl SequentialSolutionListEvaluator

.. java:import:: org.uma.jmetal.util.pseudorandom JMetalRandom

.. java:import:: org.uma.jmetal.util.pseudorandom PseudoRandomGenerator

DMOPSOBuilder
=============

.. java:package:: org.uma.jmetal.algorithm.multiobjective.dmopso
   :noindex:

.. java:type:: public class DMOPSOBuilder implements AlgorithmBuilder<DMOPSO>

   :author: Jorge Rodriguez

Constructors
------------
DMOPSOBuilder
^^^^^^^^^^^^^

.. java:constructor:: public DMOPSOBuilder(DoubleProblem problem)
   :outertype: DMOPSOBuilder

Methods
-------
build
^^^^^

.. java:method:: public DMOPSO build()
   :outertype: DMOPSOBuilder

getC1Max
^^^^^^^^

.. java:method:: public double getC1Max()
   :outertype: DMOPSOBuilder

getC1Min
^^^^^^^^

.. java:method:: public double getC1Min()
   :outertype: DMOPSOBuilder

getC2Max
^^^^^^^^

.. java:method:: public double getC2Max()
   :outertype: DMOPSOBuilder

getC2Min
^^^^^^^^

.. java:method:: public double getC2Min()
   :outertype: DMOPSOBuilder

getChangeVelocity1
^^^^^^^^^^^^^^^^^^

.. java:method:: public double getChangeVelocity1()
   :outertype: DMOPSOBuilder

getChangeVelocity2
^^^^^^^^^^^^^^^^^^

.. java:method:: public double getChangeVelocity2()
   :outertype: DMOPSOBuilder

getDataDirectory
^^^^^^^^^^^^^^^^

.. java:method:: public String getDataDirectory()
   :outertype: DMOPSOBuilder

getEvaluator
^^^^^^^^^^^^

.. java:method:: public SolutionListEvaluator<DoubleSolution> getEvaluator()
   :outertype: DMOPSOBuilder

getFunctionType
^^^^^^^^^^^^^^^

.. java:method:: public DMOPSO.FunctionType getFunctionType()
   :outertype: DMOPSOBuilder

getMaxAge
^^^^^^^^^

.. java:method:: public int getMaxAge()
   :outertype: DMOPSOBuilder

getMaxIterations
^^^^^^^^^^^^^^^^

.. java:method:: public int getMaxIterations()
   :outertype: DMOPSOBuilder

getName
^^^^^^^

.. java:method:: public String getName()
   :outertype: DMOPSOBuilder

getProblem
^^^^^^^^^^

.. java:method:: public DoubleProblem getProblem()
   :outertype: DMOPSOBuilder

getR1Max
^^^^^^^^

.. java:method:: public double getR1Max()
   :outertype: DMOPSOBuilder

getR1Min
^^^^^^^^

.. java:method:: public double getR1Min()
   :outertype: DMOPSOBuilder

getR2Max
^^^^^^^^

.. java:method:: public double getR2Max()
   :outertype: DMOPSOBuilder

getR2Min
^^^^^^^^

.. java:method:: public double getR2Min()
   :outertype: DMOPSOBuilder

getSwarmSize
^^^^^^^^^^^^

.. java:method:: public int getSwarmSize()
   :outertype: DMOPSOBuilder

getWeightMax
^^^^^^^^^^^^

.. java:method:: public double getWeightMax()
   :outertype: DMOPSOBuilder

getWeightMin
^^^^^^^^^^^^

.. java:method:: public double getWeightMin()
   :outertype: DMOPSOBuilder

setC1Max
^^^^^^^^

.. java:method:: public DMOPSOBuilder setC1Max(double c1Max)
   :outertype: DMOPSOBuilder

setC1Min
^^^^^^^^

.. java:method:: public DMOPSOBuilder setC1Min(double c1Min)
   :outertype: DMOPSOBuilder

setC2Max
^^^^^^^^

.. java:method:: public DMOPSOBuilder setC2Max(double c2Max)
   :outertype: DMOPSOBuilder

setC2Min
^^^^^^^^

.. java:method:: public DMOPSOBuilder setC2Min(double c2Min)
   :outertype: DMOPSOBuilder

setChangeVelocity1
^^^^^^^^^^^^^^^^^^

.. java:method:: public DMOPSOBuilder setChangeVelocity1(double changeVelocity1)
   :outertype: DMOPSOBuilder

setChangeVelocity2
^^^^^^^^^^^^^^^^^^

.. java:method:: public DMOPSOBuilder setChangeVelocity2(double changeVelocity2)
   :outertype: DMOPSOBuilder

setDataDirectory
^^^^^^^^^^^^^^^^

.. java:method:: public DMOPSOBuilder setDataDirectory(String dataDirectory)
   :outertype: DMOPSOBuilder

setFunctionType
^^^^^^^^^^^^^^^

.. java:method:: public DMOPSOBuilder setFunctionType(DMOPSO.FunctionType functionType)
   :outertype: DMOPSOBuilder

setMaxAge
^^^^^^^^^

.. java:method:: public DMOPSOBuilder setMaxAge(int maxAge)
   :outertype: DMOPSOBuilder

setMaxIterations
^^^^^^^^^^^^^^^^

.. java:method:: public DMOPSOBuilder setMaxIterations(int maxIterations)
   :outertype: DMOPSOBuilder

setName
^^^^^^^

.. java:method:: public DMOPSOBuilder setName(String name)
   :outertype: DMOPSOBuilder

setR1Max
^^^^^^^^

.. java:method:: public DMOPSOBuilder setR1Max(double r1Max)
   :outertype: DMOPSOBuilder

setR1Min
^^^^^^^^

.. java:method:: public DMOPSOBuilder setR1Min(double r1Min)
   :outertype: DMOPSOBuilder

setR2Max
^^^^^^^^

.. java:method:: public DMOPSOBuilder setR2Max(double r2Max)
   :outertype: DMOPSOBuilder

setR2Min
^^^^^^^^

.. java:method:: public DMOPSOBuilder setR2Min(double r2Min)
   :outertype: DMOPSOBuilder

setRandomGenerator
^^^^^^^^^^^^^^^^^^

.. java:method:: public DMOPSOBuilder setRandomGenerator(PseudoRandomGenerator randomGenerator)
   :outertype: DMOPSOBuilder

setSolutionListEvaluator
^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public DMOPSOBuilder setSolutionListEvaluator(SolutionListEvaluator<DoubleSolution> evaluator)
   :outertype: DMOPSOBuilder

setSwarmSize
^^^^^^^^^^^^

.. java:method:: public DMOPSOBuilder setSwarmSize(int swarmSize)
   :outertype: DMOPSOBuilder

setVariant
^^^^^^^^^^

.. java:method:: public DMOPSOBuilder setVariant(DMOPSOVariant variant)
   :outertype: DMOPSOBuilder

setWeightMax
^^^^^^^^^^^^

.. java:method:: public DMOPSOBuilder setWeightMax(double weightMax)
   :outertype: DMOPSOBuilder

setWeightMin
^^^^^^^^^^^^

.. java:method:: public DMOPSOBuilder setWeightMin(double weightMin)
   :outertype: DMOPSOBuilder

