.. java:import:: org.uma.jmetal.algorithm Algorithm

.. java:import:: org.uma.jmetal.algorithm.multiobjective.smpso SMPSORP

.. java:import:: org.uma.jmetal.operator MutationOperator

.. java:import:: org.uma.jmetal.operator.impl.mutation PolynomialMutation

.. java:import:: org.uma.jmetal.problem DoubleProblem

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.util AlgorithmRunner

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: org.uma.jmetal.util JMetalLogger

.. java:import:: org.uma.jmetal.util ProblemUtils

.. java:import:: org.uma.jmetal.util.archivewithreferencepoint ArchiveWithReferencePoint

.. java:import:: org.uma.jmetal.util.archivewithreferencepoint.impl CrowdingDistanceArchiveWithReferencePoint

.. java:import:: org.uma.jmetal.util.evaluator.impl SequentialSolutionListEvaluator

.. java:import:: org.uma.jmetal.util.fileoutput SolutionListOutput

.. java:import:: org.uma.jmetal.util.fileoutput.impl DefaultFileOutputContext

.. java:import:: java.io IOException

.. java:import:: java.util ArrayList

.. java:import:: java.util Arrays

.. java:import:: java.util List

SMPSORPWithOneReferencePointRunner
==================================

.. java:package:: org.uma.jmetal.runner.multiobjective
   :noindex:

.. java:type:: public class SMPSORPWithOneReferencePointRunner

Methods
-------
main
^^^^

.. java:method:: public static void main(String[] args) throws JMetalException
   :outertype: SMPSORPWithOneReferencePointRunner

   Program to run the SMPSORP algorithm with one reference point. SMPSORP is described in "Extending the Speed-constrained Multi-Objective PSO (SMPSO) With Reference Point Based Preference * Articulation. Antonio J. Nebro, Juan J. Durillo, José García-Nieto, Cristóbal Barba-González, * Javier Del Ser, Carlos A. Coello Coello, Antonio Benítez-Hidalgo, José F. Aldana-Montes. * Parallel Problem Solving from Nature -- PPSN XV. Lecture Notes In Computer Science, Vol. 11101, * pp. 298-310. 2018

   :author: Antonio J. Nebro

