.. java:import:: org.uma.jmetal.operator CrossoverOperator

.. java:import:: org.uma.jmetal.operator MutationOperator

.. java:import:: org.uma.jmetal.operator SelectionOperator

.. java:import:: org.uma.jmetal.operator.impl.selection BinaryTournamentSelection

.. java:import:: org.uma.jmetal.problem Problem

.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util AlgorithmBuilder

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: org.uma.jmetal.util.archive BoundedArchive

.. java:import:: org.uma.jmetal.util.archive.impl CrowdingDistanceArchive

.. java:import:: org.uma.jmetal.util.comparator RankingAndCrowdingDistanceComparator

.. java:import:: org.uma.jmetal.util.evaluator SolutionListEvaluator

.. java:import:: org.uma.jmetal.util.evaluator.impl SequentialSolutionListEvaluator

.. java:import:: org.uma.jmetal.util.neighborhood Neighborhood

.. java:import:: org.uma.jmetal.util.neighborhood.impl C9

.. java:import:: java.util List

MOCellBuilder
=============

.. java:package:: org.uma.jmetal.algorithm.multiobjective.mocell
   :noindex:

.. java:type:: public class MOCellBuilder<S extends Solution<?>> implements AlgorithmBuilder<MOCell<S>>

   Created by juanjo

Fields
------
archive
^^^^^^^

.. java:field:: protected BoundedArchive<S> archive
   :outertype: MOCellBuilder

crossoverOperator
^^^^^^^^^^^^^^^^^

.. java:field:: protected CrossoverOperator<S> crossoverOperator
   :outertype: MOCellBuilder

evaluator
^^^^^^^^^

.. java:field:: protected SolutionListEvaluator<S> evaluator
   :outertype: MOCellBuilder

maxEvaluations
^^^^^^^^^^^^^^

.. java:field:: protected int maxEvaluations
   :outertype: MOCellBuilder

mutationOperator
^^^^^^^^^^^^^^^^

.. java:field:: protected MutationOperator<S> mutationOperator
   :outertype: MOCellBuilder

neighborhood
^^^^^^^^^^^^

.. java:field:: protected Neighborhood<S> neighborhood
   :outertype: MOCellBuilder

populationSize
^^^^^^^^^^^^^^

.. java:field:: protected int populationSize
   :outertype: MOCellBuilder

problem
^^^^^^^

.. java:field:: protected final Problem<S> problem
   :outertype: MOCellBuilder

   MOCellBuilder class

selectionOperator
^^^^^^^^^^^^^^^^^

.. java:field:: protected SelectionOperator<List<S>, S> selectionOperator
   :outertype: MOCellBuilder

Constructors
------------
MOCellBuilder
^^^^^^^^^^^^^

.. java:constructor:: public MOCellBuilder(Problem<S> problem, CrossoverOperator<S> crossoverOperator, MutationOperator<S> mutationOperator)
   :outertype: MOCellBuilder

   MOCellBuilder constructor

Methods
-------
build
^^^^^

.. java:method:: public MOCell<S> build()
   :outertype: MOCellBuilder

getArchive
^^^^^^^^^^

.. java:method:: public BoundedArchive<S> getArchive()
   :outertype: MOCellBuilder

getCrossoverOperator
^^^^^^^^^^^^^^^^^^^^

.. java:method:: public CrossoverOperator<S> getCrossoverOperator()
   :outertype: MOCellBuilder

getMaxEvaluations
^^^^^^^^^^^^^^^^^

.. java:method:: public int getMaxEvaluations()
   :outertype: MOCellBuilder

getMutationOperator
^^^^^^^^^^^^^^^^^^^

.. java:method:: public MutationOperator<S> getMutationOperator()
   :outertype: MOCellBuilder

getPopulationSize
^^^^^^^^^^^^^^^^^

.. java:method:: public int getPopulationSize()
   :outertype: MOCellBuilder

getProblem
^^^^^^^^^^

.. java:method:: public Problem<S> getProblem()
   :outertype: MOCellBuilder

getSelectionOperator
^^^^^^^^^^^^^^^^^^^^

.. java:method:: public SelectionOperator<List<S>, S> getSelectionOperator()
   :outertype: MOCellBuilder

getSolutionListEvaluator
^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public SolutionListEvaluator<S> getSolutionListEvaluator()
   :outertype: MOCellBuilder

setArchive
^^^^^^^^^^

.. java:method:: public MOCellBuilder<S> setArchive(BoundedArchive<S> archive)
   :outertype: MOCellBuilder

setMaxEvaluations
^^^^^^^^^^^^^^^^^

.. java:method:: public MOCellBuilder<S> setMaxEvaluations(int maxEvaluations)
   :outertype: MOCellBuilder

setNeighborhood
^^^^^^^^^^^^^^^

.. java:method:: public MOCellBuilder<S> setNeighborhood(Neighborhood<S> neighborhood)
   :outertype: MOCellBuilder

setPopulationSize
^^^^^^^^^^^^^^^^^

.. java:method:: public MOCellBuilder<S> setPopulationSize(int populationSize)
   :outertype: MOCellBuilder

setSelectionOperator
^^^^^^^^^^^^^^^^^^^^

.. java:method:: public MOCellBuilder<S> setSelectionOperator(SelectionOperator<List<S>, S> selectionOperator)
   :outertype: MOCellBuilder

setSolutionListEvaluator
^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public MOCellBuilder<S> setSolutionListEvaluator(SolutionListEvaluator<S> evaluator)
   :outertype: MOCellBuilder

