.. java:import:: org.uma.jmetal.operator CrossoverOperator

.. java:import:: org.uma.jmetal.operator MutationOperator

.. java:import:: org.uma.jmetal.problem Problem

.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util AlgorithmBuilder

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: org.uma.jmetal.util.evaluator SolutionListEvaluator

.. java:import:: org.uma.jmetal.util.evaluator.impl SequentialSolutionListEvaluator

PESA2Builder
============

.. java:package:: org.uma.jmetal.algorithm.multiobjective.pesa2
   :noindex:

.. java:type:: public class PESA2Builder<S extends Solution<?>> implements AlgorithmBuilder<PESA2<S>>

   Created by Antonio J. Nebro

Constructors
------------
PESA2Builder
^^^^^^^^^^^^

.. java:constructor:: public PESA2Builder(Problem<S> problem, CrossoverOperator<S> crossoverOperator, MutationOperator<S> mutationOperator)
   :outertype: PESA2Builder

   Constructor

Methods
-------
build
^^^^^

.. java:method:: public PESA2<S> build()
   :outertype: PESA2Builder

getArchiveSize
^^^^^^^^^^^^^^

.. java:method:: public int getArchiveSize()
   :outertype: PESA2Builder

getBiSections
^^^^^^^^^^^^^

.. java:method:: public int getBiSections()
   :outertype: PESA2Builder

getCrossoverOperator
^^^^^^^^^^^^^^^^^^^^

.. java:method:: public CrossoverOperator<S> getCrossoverOperator()
   :outertype: PESA2Builder

getMaxEvaluations
^^^^^^^^^^^^^^^^^

.. java:method:: public int getMaxEvaluations()
   :outertype: PESA2Builder

getMutationOperator
^^^^^^^^^^^^^^^^^^^

.. java:method:: public MutationOperator<S> getMutationOperator()
   :outertype: PESA2Builder

getPopulationSize
^^^^^^^^^^^^^^^^^

.. java:method:: public int getPopulationSize()
   :outertype: PESA2Builder

getProblem
^^^^^^^^^^

.. java:method:: public Problem<S> getProblem()
   :outertype: PESA2Builder

getSolutionListEvaluator
^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public SolutionListEvaluator<S> getSolutionListEvaluator()
   :outertype: PESA2Builder

setArchiveSize
^^^^^^^^^^^^^^

.. java:method:: public PESA2Builder<S> setArchiveSize(int archiveSize)
   :outertype: PESA2Builder

setBisections
^^^^^^^^^^^^^

.. java:method:: public PESA2Builder<S> setBisections(int biSections)
   :outertype: PESA2Builder

setMaxEvaluations
^^^^^^^^^^^^^^^^^

.. java:method:: public PESA2Builder<S> setMaxEvaluations(int maxEvaluations)
   :outertype: PESA2Builder

setPopulationSize
^^^^^^^^^^^^^^^^^

.. java:method:: public PESA2Builder<S> setPopulationSize(int populationSize)
   :outertype: PESA2Builder

setSolutionListEvaluator
^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public PESA2Builder<S> setSolutionListEvaluator(SolutionListEvaluator<S> evaluator)
   :outertype: PESA2Builder

