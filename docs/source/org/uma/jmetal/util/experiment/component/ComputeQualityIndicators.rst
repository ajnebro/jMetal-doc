.. java:import:: org.apache.commons.lang3.tuple ImmutablePair

.. java:import:: org.apache.commons.lang3.tuple Pair

.. java:import:: org.uma.jmetal.qualityindicator QualityIndicator

.. java:import:: org.uma.jmetal.qualityindicator.impl GenericIndicator

.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: org.uma.jmetal.util JMetalLogger

.. java:import:: org.uma.jmetal.util.experiment Experiment

.. java:import:: org.uma.jmetal.util.experiment ExperimentComponent

.. java:import:: org.uma.jmetal.util.experiment.util ExperimentAlgorithm

.. java:import:: org.uma.jmetal.util.experiment.util ExperimentProblem

.. java:import:: org.uma.jmetal.util.front Front

.. java:import:: org.uma.jmetal.util.front.imp ArrayFront

.. java:import:: org.uma.jmetal.util.front.util FrontNormalizer

.. java:import:: org.uma.jmetal.util.front.util FrontUtils

.. java:import:: org.uma.jmetal.util.point PointSolution

.. java:import:: java.io File

.. java:import:: java.io FileWriter

.. java:import:: java.io IOException

.. java:import:: java.nio.charset StandardCharsets

.. java:import:: java.nio.file Files

.. java:import:: java.nio.file Path

.. java:import:: java.nio.file Paths

.. java:import:: java.util ArrayList

.. java:import:: java.util Collections

.. java:import:: java.util Comparator

.. java:import:: java.util List

ComputeQualityIndicators
========================

.. java:package:: org.uma.jmetal.util.experiment.component
   :noindex:

.. java:type:: public class ComputeQualityIndicators<S extends Solution<?>, Result> implements ExperimentComponent

   This class computes the \ :java:ref:`QualityIndicator`\ s of an experiment. Once the algorithms of an experiment have been executed through running an instance of class \ :java:ref:`ExecuteAlgorithms`\ , the list of indicators in obtained from the \ :java:ref:`#getIndicatorsList() <ExperimentComponent>`\  method. Then, for every combination algorithm + problem, the indicators are applied to all the FUN files and the resulting values are store in a file called as \ :java:ref:`#getName() <QualityIndicator>`\ , which is located in the same directory of the FUN files.

   :author: Antonio J. Nebro

Constructors
------------
ComputeQualityIndicators
^^^^^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public ComputeQualityIndicators(Experiment<S, Result> experiment)
   :outertype: ComputeQualityIndicators

Methods
-------
findBestIndicatorFronts
^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public void findBestIndicatorFronts(Experiment<?, Result> experiment) throws IOException
   :outertype: ComputeQualityIndicators

run
^^^

.. java:method:: @Override public void run() throws IOException
   :outertype: ComputeQualityIndicators

