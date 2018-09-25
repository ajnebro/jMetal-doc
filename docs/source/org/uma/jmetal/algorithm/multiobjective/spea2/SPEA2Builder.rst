.. java:import:: org.uma.jmetal.operator CrossoverOperator

.. java:import:: org.uma.jmetal.operator MutationOperator

.. java:import:: org.uma.jmetal.operator SelectionOperator

.. java:import:: org.uma.jmetal.operator.impl.selection BinaryTournamentSelection

.. java:import:: org.uma.jmetal.problem Problem

.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util AlgorithmBuilder

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: org.uma.jmetal.util.evaluator SolutionListEvaluator

.. java:import:: org.uma.jmetal.util.evaluator.impl SequentialSolutionListEvaluator

.. java:import:: java.util List

SPEA2Builder
============

.. java:package:: org.uma.jmetal.algorithm.multiobjective.spea2
   :noindex:

.. java:type:: public class SPEA2Builder<S extends Solution<?>> implements AlgorithmBuilder<SPEA2<S>>

   :author: Juan J. Durillo

Fields
------
crossoverOperator
^^^^^^^^^^^^^^^^^

.. java:field:: protected CrossoverOperator<S> crossoverOperator
   :outertype: SPEA2Builder

evaluator
^^^^^^^^^

.. java:field:: protected SolutionListEvaluator<S> evaluator
   :outertype: SPEA2Builder

maxIterations
^^^^^^^^^^^^^

.. java:field:: protected int maxIterations
   :outertype: SPEA2Builder

mutationOperator
^^^^^^^^^^^^^^^^

.. java:field:: protected MutationOperator<S> mutationOperator
   :outertype: SPEA2Builder

populationSize
^^^^^^^^^^^^^^

.. java:field:: protected int populationSize
   :outertype: SPEA2Builder

problem
^^^^^^^

.. java:field:: protected final Problem<S> problem
   :outertype: SPEA2Builder

   SPEA2Builder class

selectionOperator
^^^^^^^^^^^^^^^^^

.. java:field:: protected SelectionOperator<List<S>, S> selectionOperator
   :outertype: SPEA2Builder

Constructors
------------
SPEA2Builder
^^^^^^^^^^^^

.. java:constructor:: public SPEA2Builder(Problem<S> problem, CrossoverOperator<S> crossoverOperator, MutationOperator<S> mutationOperator)
   :outertype: SPEA2Builder

   SPEA2Builder constructor

Methods
-------
build
^^^^^

.. java:method:: public SPEA2<S> build()
   :outertype: SPEA2Builder

getCrossoverOperator
^^^^^^^^^^^^^^^^^^^^

.. java:method:: public CrossoverOperator<S> getCrossoverOperator()
   :outertype: SPEA2Builder

getMaxIterations
^^^^^^^^^^^^^^^^

.. java:method:: public int getMaxIterations()
   :outertype: SPEA2Builder

getMutationOperator
^^^^^^^^^^^^^^^^^^^

.. java:method:: public MutationOperator<S> getMutationOperator()
   :outertype: SPEA2Builder

getPopulationSize
^^^^^^^^^^^^^^^^^

.. java:method:: public int getPopulationSize()
   :outertype: SPEA2Builder

getProblem
^^^^^^^^^^

.. java:method:: public Problem<S> getProblem()
   :outertype: SPEA2Builder

getSelectionOperator
^^^^^^^^^^^^^^^^^^^^

.. java:method:: public SelectionOperator<List<S>, S> getSelectionOperator()
   :outertype: SPEA2Builder

getSolutionListEvaluator
^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public SolutionListEvaluator<S> getSolutionListEvaluator()
   :outertype: SPEA2Builder

setMaxIterations
^^^^^^^^^^^^^^^^

.. java:method:: public SPEA2Builder<S> setMaxIterations(int maxIterations)
   :outertype: SPEA2Builder

setPopulationSize
^^^^^^^^^^^^^^^^^

.. java:method:: public SPEA2Builder<S> setPopulationSize(int populationSize)
   :outertype: SPEA2Builder

setSelectionOperator
^^^^^^^^^^^^^^^^^^^^

.. java:method:: public SPEA2Builder<S> setSelectionOperator(SelectionOperator<List<S>, S> selectionOperator)
   :outertype: SPEA2Builder

setSolutionListEvaluator
^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public SPEA2Builder<S> setSolutionListEvaluator(SolutionListEvaluator<S> evaluator)
   :outertype: SPEA2Builder

