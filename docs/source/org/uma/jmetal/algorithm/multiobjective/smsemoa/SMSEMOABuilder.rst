.. java:import:: org.uma.jmetal.operator CrossoverOperator

.. java:import:: org.uma.jmetal.operator MutationOperator

.. java:import:: org.uma.jmetal.operator SelectionOperator

.. java:import:: org.uma.jmetal.operator.impl.selection RandomSelection

.. java:import:: org.uma.jmetal.problem Problem

.. java:import:: org.uma.jmetal.qualityindicator.impl Hypervolume

.. java:import:: org.uma.jmetal.qualityindicator.impl.hypervolume PISAHypervolume

.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util AlgorithmBuilder

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: org.uma.jmetal.util.comparator DominanceComparator

.. java:import:: java.util Comparator

.. java:import:: java.util List

SMSEMOABuilder
==============

.. java:package:: org.uma.jmetal.algorithm.multiobjective.smsemoa
   :noindex:

.. java:type:: public class SMSEMOABuilder<S extends Solution<?>> implements AlgorithmBuilder<SMSEMOA<S>>

   :author: Antonio J. Nebro

Fields
------
crossoverOperator
^^^^^^^^^^^^^^^^^

.. java:field:: protected CrossoverOperator<S> crossoverOperator
   :outertype: SMSEMOABuilder

dominanceComparator
^^^^^^^^^^^^^^^^^^^

.. java:field:: protected Comparator<S> dominanceComparator
   :outertype: SMSEMOABuilder

hypervolumeImplementation
^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:field:: protected Hypervolume<S> hypervolumeImplementation
   :outertype: SMSEMOABuilder

maxEvaluations
^^^^^^^^^^^^^^

.. java:field:: protected int maxEvaluations
   :outertype: SMSEMOABuilder

mutationOperator
^^^^^^^^^^^^^^^^

.. java:field:: protected MutationOperator<S> mutationOperator
   :outertype: SMSEMOABuilder

offset
^^^^^^

.. java:field:: protected double offset
   :outertype: SMSEMOABuilder

populationSize
^^^^^^^^^^^^^^

.. java:field:: protected int populationSize
   :outertype: SMSEMOABuilder

problem
^^^^^^^

.. java:field:: protected Problem<S> problem
   :outertype: SMSEMOABuilder

selectionOperator
^^^^^^^^^^^^^^^^^

.. java:field:: protected SelectionOperator<List<S>, S> selectionOperator
   :outertype: SMSEMOABuilder

Constructors
------------
SMSEMOABuilder
^^^^^^^^^^^^^^

.. java:constructor:: public SMSEMOABuilder(Problem<S> problem, CrossoverOperator<S> crossoverOperator, MutationOperator<S> mutationOperator)
   :outertype: SMSEMOABuilder

Methods
-------
build
^^^^^

.. java:method:: @Override public SMSEMOA<S> build()
   :outertype: SMSEMOABuilder

getCrossoverOperator
^^^^^^^^^^^^^^^^^^^^

.. java:method:: public CrossoverOperator<S> getCrossoverOperator()
   :outertype: SMSEMOABuilder

getMaxEvaluations
^^^^^^^^^^^^^^^^^

.. java:method:: public int getMaxEvaluations()
   :outertype: SMSEMOABuilder

getMutationOperator
^^^^^^^^^^^^^^^^^^^

.. java:method:: public MutationOperator<S> getMutationOperator()
   :outertype: SMSEMOABuilder

getOffset
^^^^^^^^^

.. java:method:: public double getOffset()
   :outertype: SMSEMOABuilder

getPopulationSize
^^^^^^^^^^^^^^^^^

.. java:method:: public int getPopulationSize()
   :outertype: SMSEMOABuilder

getProblem
^^^^^^^^^^

.. java:method:: public Problem<S> getProblem()
   :outertype: SMSEMOABuilder

getSelectionOperator
^^^^^^^^^^^^^^^^^^^^

.. java:method:: public SelectionOperator<List<S>, S> getSelectionOperator()
   :outertype: SMSEMOABuilder

setCrossoverOperator
^^^^^^^^^^^^^^^^^^^^

.. java:method:: public SMSEMOABuilder<S> setCrossoverOperator(CrossoverOperator<S> crossover)
   :outertype: SMSEMOABuilder

setDominanceComparator
^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public SMSEMOABuilder<S> setDominanceComparator(Comparator<S> dominanceComparator)
   :outertype: SMSEMOABuilder

setHypervolumeImplementation
^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public SMSEMOABuilder<S> setHypervolumeImplementation(Hypervolume<S> hypervolumeImplementation)
   :outertype: SMSEMOABuilder

setMaxEvaluations
^^^^^^^^^^^^^^^^^

.. java:method:: public SMSEMOABuilder<S> setMaxEvaluations(int maxEvaluations)
   :outertype: SMSEMOABuilder

setMutationOperator
^^^^^^^^^^^^^^^^^^^

.. java:method:: public SMSEMOABuilder<S> setMutationOperator(MutationOperator<S> mutation)
   :outertype: SMSEMOABuilder

setOffset
^^^^^^^^^

.. java:method:: public SMSEMOABuilder<S> setOffset(double offset)
   :outertype: SMSEMOABuilder

setPopulationSize
^^^^^^^^^^^^^^^^^

.. java:method:: public SMSEMOABuilder<S> setPopulationSize(int populationSize)
   :outertype: SMSEMOABuilder

setSelectionOperator
^^^^^^^^^^^^^^^^^^^^

.. java:method:: public SMSEMOABuilder<S> setSelectionOperator(SelectionOperator<List<S>, S> selection)
   :outertype: SMSEMOABuilder

