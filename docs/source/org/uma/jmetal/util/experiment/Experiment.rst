.. java:import:: org.uma.jmetal.qualityindicator.impl GenericIndicator

.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util.experiment.util ExperimentAlgorithm

.. java:import:: org.uma.jmetal.util.experiment.util ExperimentProblem

.. java:import:: java.util ArrayList

.. java:import:: java.util List

Experiment
==========

.. java:package:: org.uma.jmetal.util.experiment
   :noindex:

.. java:type:: public class Experiment<S extends Solution<?>, Result>

   Class for describing the configuration of a jMetal experiment. Created by Antonio J. Nebro on 17/07/14.

Constructors
------------
Experiment
^^^^^^^^^^

.. java:constructor:: public Experiment(ExperimentBuilder<S, Result> builder)
   :outertype: Experiment

   Constructor

Methods
-------
getAlgorithmList
^^^^^^^^^^^^^^^^

.. java:method:: public List<ExperimentAlgorithm<S, Result>> getAlgorithmList()
   :outertype: Experiment

getExperimentBaseDirectory
^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public String getExperimentBaseDirectory()
   :outertype: Experiment

getExperimentName
^^^^^^^^^^^^^^^^^

.. java:method:: public String getExperimentName()
   :outertype: Experiment

getIndependentRuns
^^^^^^^^^^^^^^^^^^

.. java:method:: public int getIndependentRuns()
   :outertype: Experiment

getIndicatorList
^^^^^^^^^^^^^^^^

.. java:method:: public List<GenericIndicator<S>> getIndicatorList()
   :outertype: Experiment

getNumberOfCores
^^^^^^^^^^^^^^^^

.. java:method:: public int getNumberOfCores()
   :outertype: Experiment

getOutputParetoFrontFileName
^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public String getOutputParetoFrontFileName()
   :outertype: Experiment

getOutputParetoSetFileName
^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public String getOutputParetoSetFileName()
   :outertype: Experiment

getProblemList
^^^^^^^^^^^^^^

.. java:method:: public List<ExperimentProblem<S>> getProblemList()
   :outertype: Experiment

getReferenceFrontDirectory
^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public String getReferenceFrontDirectory()
   :outertype: Experiment

removeDuplicatedAlgorithms
^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public void removeDuplicatedAlgorithms()
   :outertype: Experiment

   The list of algorithms contain an algorithm instance per problem. This is not convenient for calculating statistical data, because a same algorithm will appear many times. This method remove duplicated algorithms and leave only an instance of each one.

setAlgorithmList
^^^^^^^^^^^^^^^^

.. java:method:: public void setAlgorithmList(List<ExperimentAlgorithm<S, Result>> algorithmList)
   :outertype: Experiment

setReferenceFrontDirectory
^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public void setReferenceFrontDirectory(String referenceFrontDirectory)
   :outertype: Experiment

