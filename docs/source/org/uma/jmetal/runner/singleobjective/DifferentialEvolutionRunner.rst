.. java:import:: org.uma.jmetal.algorithm Algorithm

.. java:import:: org.uma.jmetal.algorithm.singleobjective.differentialevolution DifferentialEvolutionBuilder

.. java:import:: org.uma.jmetal.operator.impl.crossover DifferentialEvolutionCrossover

.. java:import:: org.uma.jmetal.operator.impl.selection DifferentialEvolutionSelection

.. java:import:: org.uma.jmetal.problem DoubleProblem

.. java:import:: org.uma.jmetal.problem.singleobjective Sphere

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.util AlgorithmRunner

.. java:import:: org.uma.jmetal.util JMetalLogger

.. java:import:: org.uma.jmetal.util.evaluator SolutionListEvaluator

.. java:import:: org.uma.jmetal.util.evaluator.impl MultithreadedSolutionListEvaluator

.. java:import:: org.uma.jmetal.util.evaluator.impl SequentialSolutionListEvaluator

.. java:import:: org.uma.jmetal.util.fileoutput SolutionListOutput

.. java:import:: org.uma.jmetal.util.fileoutput.impl DefaultFileOutputContext

.. java:import:: java.util ArrayList

.. java:import:: java.util List

DifferentialEvolutionRunner
===========================

.. java:package:: org.uma.jmetal.runner.singleobjective
   :noindex:

.. java:type:: public class DifferentialEvolutionRunner

   Class to configure and run a differential evolution algorithm. The algorithm can be configured to use threads. The number of cores is specified as an optional parameter. The target problem is Sphere.

   :author: Antonio J. Nebro

Methods
-------
main
^^^^

.. java:method:: public static void main(String[] args) throws Exception
   :outertype: DifferentialEvolutionRunner

   Usage: java org.uma.jmetal.runner.singleobjective.DifferentialEvolutionRunner [cores]

