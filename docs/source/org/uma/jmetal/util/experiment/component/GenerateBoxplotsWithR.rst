.. java:import:: org.uma.jmetal.qualityindicator.impl GenericIndicator

.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util.experiment Experiment

.. java:import:: org.uma.jmetal.util.experiment ExperimentComponent

.. java:import:: org.uma.jmetal.util.experiment.util ExperimentProblem

.. java:import:: java.io File

.. java:import:: java.io FileWriter

.. java:import:: java.io IOException

GenerateBoxplotsWithR
=====================

.. java:package:: org.uma.jmetal.util.experiment.component
   :noindex:

.. java:type:: public class GenerateBoxplotsWithR<Result> implements ExperimentComponent

   This class generates a R script that generates an eps file containing boxplots The results are a set of R files that are written in the directory \ :java:ref:`#getExperimentBaseDirectory() <Experiment>`\ /R. Each file is called as indicatorName.Wilcoxon.R To run the R script: Rscript indicatorName.Wilcoxon.R To generate the resulting Latex file: pdflatex indicatorName.Wilcoxon.tex

   :author: Antonio J. Nebro

Constructors
------------
GenerateBoxplotsWithR
^^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public GenerateBoxplotsWithR(Experiment<?, Result> experimentConfiguration)
   :outertype: GenerateBoxplotsWithR

Methods
-------
run
^^^

.. java:method:: @Override public void run() throws IOException
   :outertype: GenerateBoxplotsWithR

setColumns
^^^^^^^^^^

.. java:method:: public GenerateBoxplotsWithR<Result> setColumns(int columns)
   :outertype: GenerateBoxplotsWithR

setDisplayNotch
^^^^^^^^^^^^^^^

.. java:method:: public GenerateBoxplotsWithR<Result> setDisplayNotch()
   :outertype: GenerateBoxplotsWithR

setRows
^^^^^^^

.. java:method:: public GenerateBoxplotsWithR<Result> setRows(int rows)
   :outertype: GenerateBoxplotsWithR

