.. java:import:: org.uma.jmetal.algorithm Algorithm

.. java:import:: org.uma.jmetal.algorithm.multiobjective.smpso SMPSOBuilder

.. java:import:: org.uma.jmetal.operator MutationOperator

.. java:import:: org.uma.jmetal.operator.impl.mutation PolynomialMutation

.. java:import:: org.uma.jmetal.problem DoubleProblem

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.util AbstractAlgorithmRunner

.. java:import:: org.uma.jmetal.util AlgorithmRunner

.. java:import:: org.uma.jmetal.util JMetalLogger

.. java:import:: org.uma.jmetal.util ProblemUtils

.. java:import:: org.uma.jmetal.util.archive BoundedArchive

.. java:import:: org.uma.jmetal.util.archive.impl CrowdingDistanceArchive

.. java:import:: org.uma.jmetal.util.evaluator SolutionListEvaluator

.. java:import:: org.uma.jmetal.util.evaluator.impl MultithreadedSolutionListEvaluator

.. java:import:: java.util List

ParallelSMPSORunner
===================

.. java:package:: org.uma.jmetal.runner.multiobjective
   :noindex:

.. java:type:: public class ParallelSMPSORunner extends AbstractAlgorithmRunner

   Class for configuring and running the SMPSO algorithm (parallel version)

   :author: Antonio J. Nebro

Methods
-------
main
^^^^

.. java:method:: public static void main(String[] args) throws Exception
   :outertype: ParallelSMPSORunner

   :param args: Command line arguments. The first (optional) argument specifies the problem to solve.
   :throws org.uma.jmetal.util.JMetalException:
   :throws java.io.IOException:
   :throws SecurityException: Invoking command: java org.uma.jmetal.runner.multiobjective.ParallelSMPSORunner problemName [referenceFront]

