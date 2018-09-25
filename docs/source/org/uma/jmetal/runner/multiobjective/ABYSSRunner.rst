.. java:import:: org.uma.jmetal.algorithm Algorithm

.. java:import:: org.uma.jmetal.algorithm.multiobjective.abyss ABYSSBuilder

.. java:import:: org.uma.jmetal.problem DoubleProblem

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.util AbstractAlgorithmRunner

.. java:import:: org.uma.jmetal.util AlgorithmRunner

.. java:import:: org.uma.jmetal.util JMetalLogger

.. java:import:: org.uma.jmetal.util ProblemUtils

.. java:import:: org.uma.jmetal.util.archive Archive

.. java:import:: org.uma.jmetal.util.archive.impl CrowdingDistanceArchive

.. java:import:: java.io FileNotFoundException

.. java:import:: java.util List

ABYSSRunner
===========

.. java:package:: org.uma.jmetal.runner.multiobjective
   :noindex:

.. java:type:: public class ABYSSRunner extends AbstractAlgorithmRunner

   This class is the main program used to configure and run AbYSS, a multiobjective scatter search metaheuristics, which is described in: A.J. Nebro, F. Luna, E. Alba, B. Dorronsoro, J.J. Durillo, A. Beham "AbYSS: Adapting Scatter Search to Multiobjective Optimization." IEEE Transactions on Evolutionary Computation. Vol. 12, No. 4 (August 2008), pp. 439-457

   :author: Antonio J. Nebro

Methods
-------
main
^^^^

.. java:method:: public static void main(String[] args) throws Exception
   :outertype: ABYSSRunner

   :param args: Command line arguments.
   :throws JMetalException:
   :throws FileNotFoundException: Invoking command: java org.uma.jmetal.runner.multiobjective.AbYSSRunner problemName [referenceFront]

