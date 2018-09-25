.. java:import:: org.uma.jmetal.algorithm.multiobjective.espea.util EnergyArchive.ReplacementStrategy

.. java:import:: org.uma.jmetal.algorithm.multiobjective.espea.util ScalarizationWrapper

.. java:import:: org.uma.jmetal.algorithm.multiobjective.espea.util ScalarizationWrapper.ScalarizationType

.. java:import:: org.uma.jmetal.operator CrossoverOperator

.. java:import:: org.uma.jmetal.operator MutationOperator

.. java:import:: org.uma.jmetal.operator SelectionOperator

.. java:import:: org.uma.jmetal.operator.impl.selection RandomSelection

.. java:import:: org.uma.jmetal.problem Problem

.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util AlgorithmBuilder

.. java:import:: org.uma.jmetal.util.evaluator SolutionListEvaluator

.. java:import:: org.uma.jmetal.util.evaluator.impl SequentialSolutionListEvaluator

.. java:import:: java.util List

ESPEABuilder
============

.. java:package:: org.uma.jmetal.algorithm.multiobjective.espea
   :noindex:

.. java:type:: public class ESPEABuilder<S extends Solution<?>> implements AlgorithmBuilder<ESPEA<S>>

Constructors
------------
ESPEABuilder
^^^^^^^^^^^^

.. java:constructor:: public ESPEABuilder(Problem<S> problem, CrossoverOperator<S> crossoverOperator, MutationOperator<S> mutationOperator)
   :outertype: ESPEABuilder

Methods
-------
build
^^^^^

.. java:method:: @Override public ESPEA<S> build()
   :outertype: ESPEABuilder

getCrossoverOperator
^^^^^^^^^^^^^^^^^^^^

.. java:method:: public CrossoverOperator<S> getCrossoverOperator()
   :outertype: ESPEABuilder

   :return: the crossoverOperator

getEvaluator
^^^^^^^^^^^^

.. java:method:: public SolutionListEvaluator<S> getEvaluator()
   :outertype: ESPEABuilder

   :return: the evaluator

getFullArchiveCrossoverOperator
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public CrossoverOperator<S> getFullArchiveCrossoverOperator()
   :outertype: ESPEABuilder

   :return: the fullArchiveCrossoverOperator

getMaxEvaluations
^^^^^^^^^^^^^^^^^

.. java:method:: public int getMaxEvaluations()
   :outertype: ESPEABuilder

   :return: the maxEvaluations

getMutationOperator
^^^^^^^^^^^^^^^^^^^

.. java:method:: public MutationOperator<S> getMutationOperator()
   :outertype: ESPEABuilder

   :return: the mutationOperator

getOperationType
^^^^^^^^^^^^^^^^

.. java:method:: public ReplacementStrategy getOperationType()
   :outertype: ESPEABuilder

   :return: the replacement strategy

getPopulationSize
^^^^^^^^^^^^^^^^^

.. java:method:: public int getPopulationSize()
   :outertype: ESPEABuilder

   :return: the populationSize

getScalarization
^^^^^^^^^^^^^^^^

.. java:method:: public ScalarizationWrapper getScalarization()
   :outertype: ESPEABuilder

   :return: the scalarization

getSelectionOperator
^^^^^^^^^^^^^^^^^^^^

.. java:method:: public SelectionOperator<List<S>, S> getSelectionOperator()
   :outertype: ESPEABuilder

   :return: the selectionOperator

isNormalizeObjectives
^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public boolean isNormalizeObjectives()
   :outertype: ESPEABuilder

   :return: the normalizeObjectives

setCrossoverOperator
^^^^^^^^^^^^^^^^^^^^

.. java:method:: public void setCrossoverOperator(CrossoverOperator<S> crossoverOperator)
   :outertype: ESPEABuilder

   :param crossoverOperator: the crossoverOperator to set

setEvaluator
^^^^^^^^^^^^

.. java:method:: public void setEvaluator(SolutionListEvaluator<S> evaluator)
   :outertype: ESPEABuilder

   :param evaluator: the evaluator to set

setFullArchiveCrossoverOperator
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public void setFullArchiveCrossoverOperator(CrossoverOperator<S> fullArchiveCrossoverOperator)
   :outertype: ESPEABuilder

   :param fullArchiveCrossoverOperator: the fullArchiveCrossoverOperator to set

setMaxEvaluations
^^^^^^^^^^^^^^^^^

.. java:method:: public void setMaxEvaluations(int maxEvaluations)
   :outertype: ESPEABuilder

   :param maxEvaluations: the maxEvaluations to set

setMutationOperator
^^^^^^^^^^^^^^^^^^^

.. java:method:: public void setMutationOperator(MutationOperator<S> mutationOperator)
   :outertype: ESPEABuilder

   :param mutationOperator: the mutationOperator to set

setNormalizeObjectives
^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public void setNormalizeObjectives(boolean normalizeObjectives)
   :outertype: ESPEABuilder

   :param normalizeObjectives: the normalizeObjectives to set

setPopulationSize
^^^^^^^^^^^^^^^^^

.. java:method:: public void setPopulationSize(int populationSize)
   :outertype: ESPEABuilder

   :param populationSize: the populationSize to set

setReplacementStrategy
^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public void setReplacementStrategy(ReplacementStrategy replacementStrategy)
   :outertype: ESPEABuilder

   :param replacementStrategy: the replacement strategy to set

setScalarization
^^^^^^^^^^^^^^^^

.. java:method:: public void setScalarization(ScalarizationWrapper scalarization)
   :outertype: ESPEABuilder

   :param scalarization: the scalarization to set

setSelectionOperator
^^^^^^^^^^^^^^^^^^^^

.. java:method:: public void setSelectionOperator(SelectionOperator<List<S>, S> selectionOperator)
   :outertype: ESPEABuilder

   :param selectionOperator: the selectionOperator to set

