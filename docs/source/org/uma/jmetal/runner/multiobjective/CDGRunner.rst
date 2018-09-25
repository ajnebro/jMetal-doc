.. java:import:: java.io FileNotFoundException

.. java:import:: java.util List

.. java:import:: org.uma.jmetal.algorithm Algorithm

.. java:import:: org.uma.jmetal.algorithm.multiobjective.cdg CDGBuilder

.. java:import:: org.uma.jmetal.operator.impl.crossover DifferentialEvolutionCrossover

.. java:import:: org.uma.jmetal.problem DoubleProblem

.. java:import:: org.uma.jmetal.problem.multiobjective.glt GLT4

.. java:import:: org.uma.jmetal.util AbstractAlgorithmRunner

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.util AlgorithmRunner

.. java:import:: org.uma.jmetal.util JMetalLogger

CDGRunner
=========

.. java:package:: org.uma.jmetal.runner.multiobjective
   :noindex:

.. java:type:: public class CDGRunner extends AbstractAlgorithmRunner

   Class for configuring and running the CDG algorithm The paper and Matlab code can be download at http://xinyecai.github.io/

   :author: Feng Zhang

Methods
-------
main
^^^^

.. java:method:: public static void main(String[] args) throws FileNotFoundException, ClassNotFoundException
   :outertype: CDGRunner

   :param args: Command line arguments.
   :throws ClassNotFoundException:
   :throws SecurityException: Invoking command: java org.uma.jmetal.runner.multiobjective.CDGRunner problemName [referenceFront]

