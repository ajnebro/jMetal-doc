.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: org.uma.jmetal.util JMetalLogger

.. java:import:: org.uma.jmetal.util.experiment Experiment

.. java:import:: org.uma.jmetal.util.experiment ExperimentComponent

.. java:import:: java.io File

ExecuteAlgorithms
=================

.. java:package:: org.uma.jmetal.util.experiment.component
   :noindex:

.. java:type:: public class ExecuteAlgorithms<S extends Solution<?>, Result> implements ExperimentComponent

   This class executes the algorithms the have been configured with a instance of class \ :java:ref:`Experiment`\ . Java 8 parallel streams are used to run the algorithms in parallel.

   The result of the execution is a pair of files FUNrunId.tsv and VARrunID.tsv per experiment, which are stored in the directory \ :java:ref:`#getExperimentBaseDirectory() <Experiment>`\ /algorithmName/problemName.

   :author: Antonio J. Nebro

Constructors
------------
ExecuteAlgorithms
^^^^^^^^^^^^^^^^^

.. java:constructor:: public ExecuteAlgorithms(Experiment<S, Result> configuration)
   :outertype: ExecuteAlgorithms

   Constructor

Methods
-------
run
^^^

.. java:method:: @Override public void run()
   :outertype: ExecuteAlgorithms

