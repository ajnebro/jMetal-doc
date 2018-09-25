.. java:import:: org.uma.jmetal.algorithm Algorithm

.. java:import:: org.uma.jmetal.algorithm.multiobjective.smpso SMPSO

.. java:import:: org.uma.jmetal.algorithm.multiobjective.smpso SMPSOBuilder

.. java:import:: org.uma.jmetal.operator MutationOperator

.. java:import:: org.uma.jmetal.operator.impl.mutation PolynomialMutation

.. java:import:: org.uma.jmetal.problem DoubleProblem

.. java:import:: org.uma.jmetal.qualityindicator.impl.hypervolume WFGHypervolume

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.util AbstractAlgorithmRunner

.. java:import:: org.uma.jmetal.util AlgorithmRunner

.. java:import:: org.uma.jmetal.util JMetalLogger

.. java:import:: org.uma.jmetal.util ProblemUtils

.. java:import:: org.uma.jmetal.util.archive BoundedArchive

.. java:import:: org.uma.jmetal.util.archive.impl HypervolumeArchive

.. java:import:: org.uma.jmetal.util.evaluator.impl SequentialSolutionListEvaluator

.. java:import:: org.uma.jmetal.util.pseudorandom.impl MersenneTwisterGenerator

.. java:import:: java.util List

SMPSOHv2Runner
==============

.. java:package:: org.uma.jmetal.runner.multiobjective
   :noindex:

.. java:type:: public class SMPSOHv2Runner extends AbstractAlgorithmRunner

   Class for configuring and running the SMPSO algorithm using an HypervolumeArchive, i.e, the SMPSOhv algorithm described in: A.J Nebro, J.J. Durillo, C.A. Coello Coello. Analysis of Leader Selection Strategies in a Multi-Objective Particle Swarm Optimizer. 2013 IEEE Congress on Evolutionary Computation. June 2013 DOI: 10.1109/CEC.2013.6557955 This is a variant using the WFG Hypervolume implementation

   :author: Antonio J. Nebro

Methods
-------
main
^^^^

.. java:method:: public static void main(String[] args) throws Exception
   :outertype: SMPSOHv2Runner

   :param args: Command line arguments. The first (optional) argument specifies the problem to solve.
   :throws org.uma.jmetal.util.JMetalException:
   :throws java.io.IOException:
   :throws SecurityException: Invoking command: java org.uma.jmetal.runner.multiobjective.SMPSOHvRunner problemName [referenceFront]

