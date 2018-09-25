.. java:import:: org.uma.jmetal.algorithm Algorithm

.. java:import:: org.uma.jmetal.algorithm.multiobjective.omopso OMOPSOBuilder

.. java:import:: org.uma.jmetal.operator.impl.mutation NonUniformMutation

.. java:import:: org.uma.jmetal.operator.impl.mutation UniformMutation

.. java:import:: org.uma.jmetal.problem DoubleProblem

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.util AbstractAlgorithmRunner

.. java:import:: org.uma.jmetal.util AlgorithmRunner

.. java:import:: org.uma.jmetal.util JMetalLogger

.. java:import:: org.uma.jmetal.util ProblemUtils

.. java:import:: org.uma.jmetal.util.evaluator.impl SequentialSolutionListEvaluator

.. java:import:: java.util List

OMOPSORunner
============

.. java:package:: org.uma.jmetal.runner.multiobjective
   :noindex:

.. java:type:: public class OMOPSORunner extends AbstractAlgorithmRunner

   Class for configuring and running the OMOPSO algorithm

   :author: Antonio J. Nebro

Methods
-------
main
^^^^

.. java:method:: public static void main(String[] args) throws Exception
   :outertype: OMOPSORunner

   :param args: Command line arguments.
   :throws org.uma.jmetal.util.JMetalException:
   :throws java.io.IOException:
   :throws SecurityException: Invoking command: java org.uma.jmetal.runner.multiobjective.OMOPSORunner problemName [referenceFront]

