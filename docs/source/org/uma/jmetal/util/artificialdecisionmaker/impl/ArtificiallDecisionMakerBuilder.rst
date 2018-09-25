.. java:import:: org.uma.jmetal.algorithm InteractiveAlgorithm

.. java:import:: org.uma.jmetal.problem Problem

.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util AlgorithmBuilder

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: java.util List

ArtificiallDecisionMakerBuilder
===============================

.. java:package:: org.uma.jmetal.util.artificialdecisionmaker.impl
   :noindex:

.. java:type:: public class ArtificiallDecisionMakerBuilder<S extends Solution<?>> implements AlgorithmBuilder<ArtificialDecisionMakerDecisionTree<S>>

   :author: Antonio J. Nebro

Constructors
------------
ArtificiallDecisionMakerBuilder
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public ArtificiallDecisionMakerBuilder(Problem<S> problem, InteractiveAlgorithm<S, List<S>> algorithm)
   :outertype: ArtificiallDecisionMakerBuilder

   ArtificiallDecisionMakerBuilder constructor

Methods
-------
build
^^^^^

.. java:method:: public ArtificialDecisionMakerDecisionTree<S> build()
   :outertype: ArtificiallDecisionMakerBuilder

getMaxIterations
^^^^^^^^^^^^^^^^

.. java:method:: public int getMaxIterations()
   :outertype: ArtificiallDecisionMakerBuilder

getProblem
^^^^^^^^^^

.. java:method:: public Problem<S> getProblem()
   :outertype: ArtificiallDecisionMakerBuilder

setAlgorithm
^^^^^^^^^^^^

.. java:method:: public ArtificiallDecisionMakerBuilder<S> setAlgorithm(InteractiveAlgorithm<S, List<S>> algorithm)
   :outertype: ArtificiallDecisionMakerBuilder

setAsp
^^^^^^

.. java:method:: public ArtificiallDecisionMakerBuilder<S> setAsp(List<Double> asp)
   :outertype: ArtificiallDecisionMakerBuilder

setConsiderationProbability
^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public ArtificiallDecisionMakerBuilder<S> setConsiderationProbability(double considerationProbability)
   :outertype: ArtificiallDecisionMakerBuilder

setMaxEvaluations
^^^^^^^^^^^^^^^^^

.. java:method:: public ArtificiallDecisionMakerBuilder<S> setMaxEvaluations(int maxEvaluations)
   :outertype: ArtificiallDecisionMakerBuilder

setNumberReferencePoints
^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public ArtificiallDecisionMakerBuilder<S> setNumberReferencePoints(int numberReferencePoints)
   :outertype: ArtificiallDecisionMakerBuilder

setRankingCoeficient
^^^^^^^^^^^^^^^^^^^^

.. java:method:: public ArtificiallDecisionMakerBuilder<S> setRankingCoeficient(List<Double> rankingCoeficient)
   :outertype: ArtificiallDecisionMakerBuilder

setTolerance
^^^^^^^^^^^^

.. java:method:: public ArtificiallDecisionMakerBuilder<S> setTolerance(double tolerance)
   :outertype: ArtificiallDecisionMakerBuilder

