.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: weka.classifiers Classifier

.. java:import:: weka.classifiers Evaluation

.. java:import:: weka.classifiers.trees J48

.. java:import:: weka.core Attribute

.. java:import:: weka.core DenseInstance

.. java:import:: weka.core Instance

.. java:import:: weka.core Instances

.. java:import:: weka.filters Filter

.. java:import:: weka.filters.unsupervised.attribute StringToWordVector

.. java:import:: java.util ArrayList

.. java:import:: java.util List

DecisionTreeEstimator
=====================

.. java:package:: org.uma.jmetal.util.artificialdecisionmaker
   :noindex:

.. java:type:: public class DecisionTreeEstimator<S extends Solution<?>>

Constructors
------------
DecisionTreeEstimator
^^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public DecisionTreeEstimator(List<S> solutionList)
   :outertype: DecisionTreeEstimator

Methods
-------
doPrediction
^^^^^^^^^^^^

.. java:method:: public double doPrediction(int index, S testSolution)
   :outertype: DecisionTreeEstimator

doPredictionVariable
^^^^^^^^^^^^^^^^^^^^

.. java:method:: public double doPredictionVariable(int index, S testSolution)
   :outertype: DecisionTreeEstimator

