.. java:import:: org.uma.jmetal.qualityindicator.impl GenericIndicator

.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util.experiment.util ExperimentAlgorithm

.. java:import:: org.uma.jmetal.util.experiment.util ExperimentProblem

.. java:import:: java.util ArrayList

.. java:import:: java.util List

ExperimentBuilder
=================

.. java:package:: org.uma.jmetal.util.experiment
   :noindex:

.. java:type:: public class ExperimentBuilder<S extends Solution<?>, Result>

   Builder for class \ :java:ref:`Experiment`\

   :author: Antonio J. Nebro

Constructors
------------
ExperimentBuilder
^^^^^^^^^^^^^^^^^

.. java:constructor:: public ExperimentBuilder(String experimentName)
   :outertype: ExperimentBuilder

Methods
-------
build
^^^^^

.. java:method:: public Experiment<S, Result> build()
   :outertype: ExperimentBuilder

getAlgorithmList
^^^^^^^^^^^^^^^^

.. java:method:: public List<ExperimentAlgorithm<S, Result>> getAlgorithmList()
   :outertype: ExperimentBuilder

getExperimentBaseDirectory
^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public String getExperimentBaseDirectory()
   :outertype: ExperimentBuilder

getExperimentName
^^^^^^^^^^^^^^^^^

.. java:method:: public String getExperimentName()
   :outertype: ExperimentBuilder

getIndependentRuns
^^^^^^^^^^^^^^^^^^

.. java:method:: public int getIndependentRuns()
   :outertype: ExperimentBuilder

getIndicatorList
^^^^^^^^^^^^^^^^

.. java:method:: public List<GenericIndicator<S>> getIndicatorList()
   :outertype: ExperimentBuilder

getNumberOfCores
^^^^^^^^^^^^^^^^

.. java:method:: public int getNumberOfCores()
   :outertype: ExperimentBuilder

getOutputParetoFrontFileName
^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public String getOutputParetoFrontFileName()
   :outertype: ExperimentBuilder

getOutputParetoSetFileName
^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public String getOutputParetoSetFileName()
   :outertype: ExperimentBuilder

getProblemList
^^^^^^^^^^^^^^

.. java:method:: public List<ExperimentProblem<S>> getProblemList()
   :outertype: ExperimentBuilder

getReferenceFrontDirectory
^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public String getReferenceFrontDirectory()
   :outertype: ExperimentBuilder

setAlgorithmList
^^^^^^^^^^^^^^^^

.. java:method:: public ExperimentBuilder<S, Result> setAlgorithmList(List<ExperimentAlgorithm<S, Result>> algorithmList)
   :outertype: ExperimentBuilder

setExperimentBaseDirectory
^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public ExperimentBuilder<S, Result> setExperimentBaseDirectory(String experimentBaseDirectory)
   :outertype: ExperimentBuilder

setIndependentRuns
^^^^^^^^^^^^^^^^^^

.. java:method:: public ExperimentBuilder<S, Result> setIndependentRuns(int independentRuns)
   :outertype: ExperimentBuilder

setIndicatorList
^^^^^^^^^^^^^^^^

.. java:method:: public ExperimentBuilder<S, Result> setIndicatorList(List<GenericIndicator<S>> indicatorList)
   :outertype: ExperimentBuilder

setNumberOfCores
^^^^^^^^^^^^^^^^

.. java:method:: public ExperimentBuilder<S, Result> setNumberOfCores(int numberOfCores)
   :outertype: ExperimentBuilder

setOutputParetoFrontFileName
^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public ExperimentBuilder<S, Result> setOutputParetoFrontFileName(String outputParetoFrontFileName)
   :outertype: ExperimentBuilder

setOutputParetoSetFileName
^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public ExperimentBuilder<S, Result> setOutputParetoSetFileName(String outputParetoSetFileName)
   :outertype: ExperimentBuilder

setProblemList
^^^^^^^^^^^^^^

.. java:method:: public ExperimentBuilder<S, Result> setProblemList(List<ExperimentProblem<S>> problemList)
   :outertype: ExperimentBuilder

setReferenceFrontDirectory
^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public ExperimentBuilder<S, Result> setReferenceFrontDirectory(String referenceFrontDirectory)
   :outertype: ExperimentBuilder

