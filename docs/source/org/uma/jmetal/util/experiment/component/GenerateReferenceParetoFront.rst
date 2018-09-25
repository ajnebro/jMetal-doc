.. java:import:: org.uma.jmetal.util JMetalLogger

.. java:import:: org.uma.jmetal.util.archive.impl NonDominatedSolutionListArchive

.. java:import:: org.uma.jmetal.util.experiment Experiment

.. java:import:: org.uma.jmetal.util.experiment ExperimentComponent

.. java:import:: org.uma.jmetal.util.experiment.util ExperimentAlgorithm

.. java:import:: org.uma.jmetal.util.experiment.util ExperimentProblem

.. java:import:: org.uma.jmetal.util.fileoutput SolutionListOutput

.. java:import:: org.uma.jmetal.util.front Front

.. java:import:: org.uma.jmetal.util.front.imp ArrayFront

.. java:import:: org.uma.jmetal.util.front.util FrontUtils

.. java:import:: org.uma.jmetal.util.point PointSolution

.. java:import:: org.uma.jmetal.util.solutionattribute.impl GenericSolutionAttribute

.. java:import:: java.io File

.. java:import:: java.io IOException

.. java:import:: java.util ArrayList

.. java:import:: java.util LinkedList

.. java:import:: java.util List

GenerateReferenceParetoFront
============================

.. java:package:: org.uma.jmetal.util.experiment.component
   :noindex:

.. java:type:: public class GenerateReferenceParetoFront implements ExperimentComponent

   This class computes a reference Pareto front from a set of files. Once the algorithms of an experiment have been executed through running an instance of class \ :java:ref:`ExecuteAlgorithms`\ , all the obtained fronts of all the algorithms are gathered per problem; then, the dominated solutions are removed and the final result is a file per problem containing the reference Pareto front. By default, the files are stored in a directory called "referenceFront", which is located in the experiment base directory. Each front is named following the scheme "problemName.rf".

   :author: Antonio J. Nebro

Constructors
------------
GenerateReferenceParetoFront
^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public GenerateReferenceParetoFront(Experiment<?, ?> experimentConfiguration)
   :outertype: GenerateReferenceParetoFront

Methods
-------
run
^^^

.. java:method:: @Override public void run() throws IOException
   :outertype: GenerateReferenceParetoFront

   The run() method creates de output directory and compute the fronts

