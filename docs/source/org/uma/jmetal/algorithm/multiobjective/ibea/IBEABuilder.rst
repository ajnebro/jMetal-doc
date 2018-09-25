.. java:import:: org.uma.jmetal.operator CrossoverOperator

.. java:import:: org.uma.jmetal.operator MutationOperator

.. java:import:: org.uma.jmetal.operator SelectionOperator

.. java:import:: org.uma.jmetal.operator.impl.crossover SBXCrossover

.. java:import:: org.uma.jmetal.operator.impl.mutation PolynomialMutation

.. java:import:: org.uma.jmetal.operator.impl.selection BinaryTournamentSelection

.. java:import:: org.uma.jmetal.problem Problem

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.util AlgorithmBuilder

.. java:import:: java.util List

IBEABuilder
===========

.. java:package:: org.uma.jmetal.algorithm.multiobjective.ibea
   :noindex:

.. java:type:: public class IBEABuilder implements AlgorithmBuilder<IBEA<DoubleSolution>>

   This class implements the IBEA algorithm

Constructors
------------
IBEABuilder
^^^^^^^^^^^

.. java:constructor:: public IBEABuilder(Problem<DoubleSolution> problem)
   :outertype: IBEABuilder

   Constructor

   :param problem:

Methods
-------
build
^^^^^

.. java:method:: public IBEA<DoubleSolution> build()
   :outertype: IBEABuilder

getArchiveSize
^^^^^^^^^^^^^^

.. java:method:: public int getArchiveSize()
   :outertype: IBEABuilder

getCrossover
^^^^^^^^^^^^

.. java:method:: public CrossoverOperator<DoubleSolution> getCrossover()
   :outertype: IBEABuilder

getMaxEvaluations
^^^^^^^^^^^^^^^^^

.. java:method:: public int getMaxEvaluations()
   :outertype: IBEABuilder

getMutation
^^^^^^^^^^^

.. java:method:: public MutationOperator<DoubleSolution> getMutation()
   :outertype: IBEABuilder

getPopulationSize
^^^^^^^^^^^^^^^^^

.. java:method:: public int getPopulationSize()
   :outertype: IBEABuilder

getSelection
^^^^^^^^^^^^

.. java:method:: public SelectionOperator<List<DoubleSolution>, DoubleSolution> getSelection()
   :outertype: IBEABuilder

setArchiveSize
^^^^^^^^^^^^^^

.. java:method:: public IBEABuilder setArchiveSize(int archiveSize)
   :outertype: IBEABuilder

setCrossover
^^^^^^^^^^^^

.. java:method:: public IBEABuilder setCrossover(CrossoverOperator<DoubleSolution> crossover)
   :outertype: IBEABuilder

setMaxEvaluations
^^^^^^^^^^^^^^^^^

.. java:method:: public IBEABuilder setMaxEvaluations(int maxEvaluations)
   :outertype: IBEABuilder

setMutation
^^^^^^^^^^^

.. java:method:: public IBEABuilder setMutation(MutationOperator<DoubleSolution> mutation)
   :outertype: IBEABuilder

setPopulationSize
^^^^^^^^^^^^^^^^^

.. java:method:: public IBEABuilder setPopulationSize(int populationSize)
   :outertype: IBEABuilder

setSelection
^^^^^^^^^^^^

.. java:method:: public IBEABuilder setSelection(SelectionOperator<List<DoubleSolution>, DoubleSolution> selection)
   :outertype: IBEABuilder

