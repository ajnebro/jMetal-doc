.. java:import:: org.apache.commons.lang3.tuple ImmutablePair

.. java:import:: org.apache.commons.lang3.tuple MutablePair

.. java:import:: org.apache.commons.lang3.tuple Pair

.. java:import:: org.uma.jmetal.qualityindicator.impl GenericIndicator

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: org.uma.jmetal.util.experiment Experiment

.. java:import:: org.uma.jmetal.util.experiment ExperimentComponent

GenerateFriedmanTestTables
==========================

.. java:package:: org.uma.jmetal.util.experiment.component
   :noindex:

.. java:type:: public class GenerateFriedmanTestTables<Result> implements ExperimentComponent

   This class computes the Friedman test ranking and generates a Latex script that produces a table per quality indicator containing the ranking The results are a set of Latex files that are written in the directory \ :java:ref:`#getExperimentBaseDirectory() <Experiment>`\ /latex. Each file is called as FriedmanTest[indicatorName].tex The implementation is based on the one included in Keel: J. Alcalá-Fdez, L. Sánchez, S. García, M.J. del Jesus, S. Ventura, J.M. Garrell, J. Otero, C. Romero, J. Bacardit, V.M. Rivas, J.C. Fernández, F. Herrera. KEEL: A Software Tool to Assess Evolutionary Algorithms to Data Mining Problems. Soft Computing 13:3 (2009) 307-318 Doi: 10.1007/s00500-008-0323-y

   :author: Antonio J. Nebro

Constructors
------------
GenerateFriedmanTestTables
^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public GenerateFriedmanTestTables(Experiment<?, Result> experimentConfiguration)
   :outertype: GenerateFriedmanTestTables

Methods
-------
prepareFileOutputContents
^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public String prepareFileOutputContents(double[] averageRanking)
   :outertype: GenerateFriedmanTestTables

run
^^^

.. java:method:: @Override public void run() throws IOException
   :outertype: GenerateFriedmanTestTables

