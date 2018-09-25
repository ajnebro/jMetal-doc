.. java:import:: org.uma.jmetal.algorithm Algorithm

.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util JMetalLogger

.. java:import:: org.uma.jmetal.util.experiment Experiment

.. java:import:: org.uma.jmetal.util.fileoutput SolutionListOutput

.. java:import:: org.uma.jmetal.util.fileoutput.impl DefaultFileOutputContext

.. java:import:: java.io File

.. java:import:: java.util List

ExperimentAlgorithm
===================

.. java:package:: org.uma.jmetal.util.experiment.util
   :noindex:

.. java:type:: public class ExperimentAlgorithm<S extends Solution<?>, Result>

   Class defining tasks for the execution of algorithms in parallel.

   :author: Antonio J. Nebro

Constructors
------------
ExperimentAlgorithm
^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public ExperimentAlgorithm(Algorithm<Result> algorithm, String algorithmTag, ExperimentProblem<S> problem, int runId)
   :outertype: ExperimentAlgorithm

   Constructor

ExperimentAlgorithm
^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public ExperimentAlgorithm(Algorithm<Result> algorithm, ExperimentProblem<S> problem, int runId)
   :outertype: ExperimentAlgorithm

Methods
-------
getAlgorithm
^^^^^^^^^^^^

.. java:method:: public Algorithm<Result> getAlgorithm()
   :outertype: ExperimentAlgorithm

getAlgorithmTag
^^^^^^^^^^^^^^^

.. java:method:: public String getAlgorithmTag()
   :outertype: ExperimentAlgorithm

getProblemTag
^^^^^^^^^^^^^

.. java:method:: public String getProblemTag()
   :outertype: ExperimentAlgorithm

getReferenceParetoFront
^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public String getReferenceParetoFront()
   :outertype: ExperimentAlgorithm

getRunId
^^^^^^^^

.. java:method:: public int getRunId()
   :outertype: ExperimentAlgorithm

runAlgorithm
^^^^^^^^^^^^

.. java:method:: public void runAlgorithm(Experiment<?, ?> experimentData)
   :outertype: ExperimentAlgorithm

