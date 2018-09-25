.. java:import:: org.uma.jmetal.algorithm Algorithm

.. java:import:: org.uma.jmetal.algorithm.multiobjective.smpso SMPSOBuilder

.. java:import:: org.uma.jmetal.operator MutationOperator

.. java:import:: org.uma.jmetal.operator.impl.mutation PolynomialMutation

.. java:import:: org.uma.jmetal.problem DoubleProblem

.. java:import:: org.uma.jmetal.problem.singleobjective Rosenbrock

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.util AbstractAlgorithmRunner

.. java:import:: org.uma.jmetal.util AlgorithmRunner

.. java:import:: org.uma.jmetal.util JMetalLogger

.. java:import:: org.uma.jmetal.util.archive BoundedArchive

.. java:import:: org.uma.jmetal.util.archive.impl CrowdingDistanceArchive

.. java:import:: org.uma.jmetal.util.evaluator.impl SequentialSolutionListEvaluator

.. java:import:: org.uma.jmetal.util.fileoutput SolutionListOutput

.. java:import:: org.uma.jmetal.util.fileoutput.impl DefaultFileOutputContext

.. java:import:: org.uma.jmetal.util.pseudorandom.impl MersenneTwisterGenerator

.. java:import:: java.util List

SMPSORunner
===========

.. java:package:: org.uma.jmetal.runner.singleobjective
   :noindex:

.. java:type:: public class SMPSORunner extends AbstractAlgorithmRunner

   Class for configuring and running the SMPSO algorithm to solve a single-objective problem

   :author: Antonio J. Nebro

Methods
-------
main
^^^^

.. java:method:: public static void main(String[] args) throws Exception
   :outertype: SMPSORunner

   :param args: Command line arguments. The first (optional) argument specifies the problem to solve.
   :throws org.uma.jmetal.util.JMetalException:
   :throws java.io.IOException:
   :throws SecurityException: Invoking command: java org.uma.jmetal.runner.multiobjective.SMPSORunner problemName [referenceFront]

