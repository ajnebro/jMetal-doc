.. java:import:: org.uma.jmetal.algorithm Algorithm

.. java:import:: org.uma.jmetal.algorithm.multiobjective.nsgaiii NSGAIIIBuilder

.. java:import:: org.uma.jmetal.operator CrossoverOperator

.. java:import:: org.uma.jmetal.operator MutationOperator

.. java:import:: org.uma.jmetal.operator SelectionOperator

.. java:import:: org.uma.jmetal.operator.impl.crossover SBXCrossover

.. java:import:: org.uma.jmetal.operator.impl.mutation PolynomialMutation

.. java:import:: org.uma.jmetal.operator.impl.selection BinaryTournamentSelection

.. java:import:: org.uma.jmetal.problem Problem

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.util.fileoutput SolutionListOutput

.. java:import:: org.uma.jmetal.util.fileoutput.impl DefaultFileOutputContext

.. java:import:: java.util List

NSGAIIIRunner
=============

.. java:package:: org.uma.jmetal.runner.multiobjective
   :noindex:

.. java:type:: public class NSGAIIIRunner extends AbstractAlgorithmRunner

   Class to configure and run the NSGA-III algorithm

Methods
-------
main
^^^^

.. java:method:: public static void main(String[] args) throws JMetalException
   :outertype: NSGAIIIRunner

   :param args: Command line arguments.
   :throws java.io.IOException:
   :throws SecurityException:
   :throws ClassNotFoundException: Usage: three options - org.uma.jmetal.runner.multiobjective.NSGAIIIRunner - org.uma.jmetal.runner.multiobjective.NSGAIIIRunner problemName - org.uma.jmetal.runner.multiobjective.NSGAIIIRunner problemName paretoFrontFile

