.. java:import:: org.apache.commons.lang3 StringUtils

.. java:import:: org.apache.commons.math3.stat.descriptive DescriptiveStatistics

.. java:import:: org.uma.jmetal.util JMetalLogger

.. java:import:: org.uma.jmetal.util.experiment Experiment

.. java:import:: org.uma.jmetal.util.experiment ExperimentComponent

GenerateLatexTablesWithStatistics
=================================

.. java:package:: org.uma.jmetal.util.experiment.component
   :noindex:

.. java:type:: public class GenerateLatexTablesWithStatistics implements ExperimentComponent

   This class computes a number of statistical values (mean, median, standard deviation, interquartile range) from the indicator files generated after executing \ :java:ref:`ExecuteAlgorithms`\  and \ :java:ref:`ComputeQualityIndicators`\ . After reading the data files and calculating the values, a Latex file is created containing an script that generates tables with the best and second best values per indicator. The name of the file is \ :java:ref:`#getExperimentName() <Experiment>`\ .tex, which is located by default in the directory \ :java:ref:`#getExperimentBaseDirectory() <Experiment>`\ /latex Although the maximum, minimum, and total number of items are also computed, no tables are generated with them (this is a pending work).

   :author: Antonio J. Nebro

Constructors
------------
GenerateLatexTablesWithStatistics
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public GenerateLatexTablesWithStatistics(Experiment<?, ?> configuration)
   :outertype: GenerateLatexTablesWithStatistics

Methods
-------
printEndLatexCommands
^^^^^^^^^^^^^^^^^^^^^

.. java:method::  void printEndLatexCommands(String fileName) throws IOException
   :outertype: GenerateLatexTablesWithStatistics

printHeaderLatexCommands
^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method::  void printHeaderLatexCommands(String fileName) throws IOException
   :outertype: GenerateLatexTablesWithStatistics

run
^^^

.. java:method:: @Override public void run() throws IOException
   :outertype: GenerateLatexTablesWithStatistics

