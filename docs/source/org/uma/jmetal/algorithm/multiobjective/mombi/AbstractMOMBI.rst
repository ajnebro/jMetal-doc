.. java:import:: org.uma.jmetal.algorithm.impl AbstractGeneticAlgorithm

.. java:import:: org.uma.jmetal.operator CrossoverOperator

.. java:import:: org.uma.jmetal.operator MutationOperator

.. java:import:: org.uma.jmetal.operator SelectionOperator

.. java:import:: org.uma.jmetal.problem Problem

.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util.evaluator SolutionListEvaluator

.. java:import:: org.uma.jmetal.util.pseudorandom JMetalRandom

.. java:import:: java.util ArrayList

.. java:import:: java.util List

AbstractMOMBI
=============

.. java:package:: org.uma.jmetal.algorithm.multiobjective.mombi
   :noindex:

.. java:type:: @SuppressWarnings public abstract class AbstractMOMBI<S extends Solution<?>> extends AbstractGeneticAlgorithm<S, List<S>>

   Abstract class representing variants of the MOMBI algorithm

   :author: Juan J. Durillo Modified by Antonio J. Nebro
   :param <S>:

Fields
------
evaluator
^^^^^^^^^

.. java:field:: protected final SolutionListEvaluator<S> evaluator
   :outertype: AbstractMOMBI

iterations
^^^^^^^^^^

.. java:field:: protected int iterations
   :outertype: AbstractMOMBI

maxIterations
^^^^^^^^^^^^^

.. java:field:: protected final int maxIterations
   :outertype: AbstractMOMBI

nadirPoint
^^^^^^^^^^

.. java:field:: protected final List<Double> nadirPoint
   :outertype: AbstractMOMBI

referencePoint
^^^^^^^^^^^^^^

.. java:field:: protected final List<Double> referencePoint
   :outertype: AbstractMOMBI

Constructors
------------
AbstractMOMBI
^^^^^^^^^^^^^

.. java:constructor:: public AbstractMOMBI(Problem<S> problem, int maxIterations, CrossoverOperator<S> crossover, MutationOperator<S> mutation, SelectionOperator<List<S>, S> selection, SolutionListEvaluator<S> evaluator)
   :outertype: AbstractMOMBI

   Constructor

   :param problem: Problem to be solved
   :param maxIterations: Maximum number of iterations the algorithm will perform
   :param crossover: Crossover operator
   :param mutation: Mutation operator
   :param selection: Selection operator
   :param evaluator: Evaluator object for evaluating solution lists

Methods
-------
evaluatePopulation
^^^^^^^^^^^^^^^^^^

.. java:method:: @Override protected List<S> evaluatePopulation(List<S> population)
   :outertype: AbstractMOMBI

getNadirPoint
^^^^^^^^^^^^^

.. java:method:: public List<Double> getNadirPoint()
   :outertype: AbstractMOMBI

getReferencePoint
^^^^^^^^^^^^^^^^^

.. java:method:: public List<Double> getReferencePoint()
   :outertype: AbstractMOMBI

getResult
^^^^^^^^^

.. java:method:: @Override public List<S> getResult()
   :outertype: AbstractMOMBI

initProgress
^^^^^^^^^^^^

.. java:method:: @Override protected void initProgress()
   :outertype: AbstractMOMBI

isStoppingConditionReached
^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override protected boolean isStoppingConditionReached()
   :outertype: AbstractMOMBI

populationIsNotFull
^^^^^^^^^^^^^^^^^^^

.. java:method:: protected boolean populationIsNotFull(List<S> population)
   :outertype: AbstractMOMBI

reproduction
^^^^^^^^^^^^

.. java:method:: @Override protected List<S> reproduction(List<S> population)
   :outertype: AbstractMOMBI

run
^^^

.. java:method:: @Override public void run()
   :outertype: AbstractMOMBI

selection
^^^^^^^^^

.. java:method:: @Override protected List<S> selection(List<S> population)
   :outertype: AbstractMOMBI

setReferencePointValue
^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: protected void setReferencePointValue(Double value, int index)
   :outertype: AbstractMOMBI

specificMOEAComputations
^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public abstract void specificMOEAComputations()
   :outertype: AbstractMOMBI

updateNadirPoint
^^^^^^^^^^^^^^^^

.. java:method:: protected void updateNadirPoint(S s)
   :outertype: AbstractMOMBI

updateNadirPoint
^^^^^^^^^^^^^^^^

.. java:method:: public void updateNadirPoint(List<S> population)
   :outertype: AbstractMOMBI

updateProgress
^^^^^^^^^^^^^^

.. java:method:: @Override protected void updateProgress()
   :outertype: AbstractMOMBI

updateReferencePoint
^^^^^^^^^^^^^^^^^^^^

.. java:method:: protected void updateReferencePoint(S s)
   :outertype: AbstractMOMBI

updateReferencePoint
^^^^^^^^^^^^^^^^^^^^

.. java:method:: public void updateReferencePoint(List<S> population)
   :outertype: AbstractMOMBI

