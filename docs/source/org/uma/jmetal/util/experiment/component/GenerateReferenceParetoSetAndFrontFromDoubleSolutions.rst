.. java:import:: org.uma.jmetal.problem DoubleProblem

.. java:import:: org.uma.jmetal.problem.impl AbstractDoubleProblem

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.solution.impl DefaultDoubleSolution

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: org.uma.jmetal.util JMetalLogger

.. java:import:: org.uma.jmetal.util.archive.impl NonDominatedSolutionListArchive

.. java:import:: org.uma.jmetal.util.experiment Experiment

.. java:import:: org.uma.jmetal.util.experiment ExperimentComponent

.. java:import:: org.uma.jmetal.util.experiment.util ExperimentAlgorithm

.. java:import:: org.uma.jmetal.util.experiment.util ExperimentProblem

.. java:import:: org.uma.jmetal.util.fileoutput SolutionListOutput

.. java:import:: org.uma.jmetal.util.front Front

.. java:import:: org.uma.jmetal.util.front.imp ArrayFront

.. java:import:: org.uma.jmetal.util.solutionattribute.impl GenericSolutionAttribute

.. java:import:: java.io File

.. java:import:: java.io FileNotFoundException

.. java:import:: java.io IOException

.. java:import:: java.util ArrayList

.. java:import:: java.util LinkedList

.. java:import:: java.util List

.. java:import:: java.util.stream Collectors

GenerateReferenceParetoSetAndFrontFromDoubleSolutions
=====================================================

.. java:package:: org.uma.jmetal.util.experiment.component
   :noindex:

.. java:type:: public class GenerateReferenceParetoSetAndFrontFromDoubleSolutions implements ExperimentComponent

   This class computes the reference Pareto set and front from a set of data files containing the variable (VARx.tsv file) and objective (FUNx.tsv) values. A requirement is that the variable values MUST correspond to \ :java:ref:`DoubleSolution`\  solutions, i.e., the solved problems must be instances of \ :java:ref:`DoubleProblem`\ . Once the algorithms of an experiment have been executed through running an instance of class \ :java:ref:`ExecuteAlgorithms`\ , all the obtained fronts of all the algorithms are gathered per problem; then, the dominated solutions are removed thus yielding to the reference Pareto front. By default, the files are stored in a directory called "referenceFront", which is located in the experiment base directory. The following files are generated per problem: - "problemName.pf": the reference Pareto front. - "problemName.ps": the reference Pareto set (i.e., the variable values of the solutions of the reference Pareto front. - "problemName.algorithmName.pf": the objectives values of the contributed solutions by the algorithm called "algorithmName" to "problemName.pf" - "problemName.algorithmName.ps": the variable values of the contributed solutions by the algorithm called "algorithmName" to "problemName.ps"

   :author: Antonio J. Nebro

Constructors
------------
GenerateReferenceParetoSetAndFrontFromDoubleSolutions
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public GenerateReferenceParetoSetAndFrontFromDoubleSolutions(Experiment<?, ?> experimentConfiguration)
   :outertype: GenerateReferenceParetoSetAndFrontFromDoubleSolutions

Methods
-------
run
^^^

.. java:method:: @Override public void run() throws IOException
   :outertype: GenerateReferenceParetoSetAndFrontFromDoubleSolutions

   The run() method creates de output directory and compute the fronts

