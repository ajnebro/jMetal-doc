.. java:import:: org.uma.jmetal.operator MutationOperator

.. java:import:: org.uma.jmetal.operator.impl.mutation NonUniformMutation

.. java:import:: org.uma.jmetal.operator.impl.mutation UniformMutation

.. java:import:: org.uma.jmetal.problem DoubleProblem

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.util AlgorithmBuilder

.. java:import:: org.uma.jmetal.util.evaluator SolutionListEvaluator

OMOPSOBuilder
=============

.. java:package:: org.uma.jmetal.algorithm.multiobjective.omopso
   :noindex:

.. java:type:: public class OMOPSOBuilder implements AlgorithmBuilder<OMOPSO>

   Class implementing the OMOPSO algorithm

Fields
------
evaluator
^^^^^^^^^

.. java:field:: protected SolutionListEvaluator<DoubleSolution> evaluator
   :outertype: OMOPSOBuilder

problem
^^^^^^^

.. java:field:: protected DoubleProblem problem
   :outertype: OMOPSOBuilder

Constructors
------------
OMOPSOBuilder
^^^^^^^^^^^^^

.. java:constructor:: public OMOPSOBuilder(DoubleProblem problem, SolutionListEvaluator<DoubleSolution> evaluator)
   :outertype: OMOPSOBuilder

Methods
-------
build
^^^^^

.. java:method:: public OMOPSO build()
   :outertype: OMOPSOBuilder

getArchiveSize
^^^^^^^^^^^^^^

.. java:method:: public int getArchiveSize()
   :outertype: OMOPSOBuilder

getMaxIterations
^^^^^^^^^^^^^^^^

.. java:method:: public int getMaxIterations()
   :outertype: OMOPSOBuilder

getNonUniformMutation
^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public NonUniformMutation getNonUniformMutation()
   :outertype: OMOPSOBuilder

getSwarmSize
^^^^^^^^^^^^

.. java:method:: public int getSwarmSize()
   :outertype: OMOPSOBuilder

getUniformMutation
^^^^^^^^^^^^^^^^^^

.. java:method:: public UniformMutation getUniformMutation()
   :outertype: OMOPSOBuilder

setArchiveSize
^^^^^^^^^^^^^^

.. java:method:: public OMOPSOBuilder setArchiveSize(int archiveSize)
   :outertype: OMOPSOBuilder

setMaxIterations
^^^^^^^^^^^^^^^^

.. java:method:: public OMOPSOBuilder setMaxIterations(int maxIterations)
   :outertype: OMOPSOBuilder

setNonUniformMutation
^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public OMOPSOBuilder setNonUniformMutation(MutationOperator<DoubleSolution> nonUniformMutation)
   :outertype: OMOPSOBuilder

setSwarmSize
^^^^^^^^^^^^

.. java:method:: public OMOPSOBuilder setSwarmSize(int swarmSize)
   :outertype: OMOPSOBuilder

setUniformMutation
^^^^^^^^^^^^^^^^^^

.. java:method:: public OMOPSOBuilder setUniformMutation(MutationOperator<DoubleSolution> uniformMutation)
   :outertype: OMOPSOBuilder

