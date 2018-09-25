.. java:import:: org.uma.jmetal.algorithm.impl AbstractGeneticAlgorithm

.. java:import:: org.uma.jmetal.algorithm.multiobjective.spea2.util EnvironmentalSelection

.. java:import:: org.uma.jmetal.operator CrossoverOperator

.. java:import:: org.uma.jmetal.operator MutationOperator

.. java:import:: org.uma.jmetal.operator SelectionOperator

.. java:import:: org.uma.jmetal.problem Problem

.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util.evaluator SolutionListEvaluator

.. java:import:: org.uma.jmetal.util.solutionattribute.impl StrengthRawFitness

.. java:import:: java.util ArrayList

.. java:import:: java.util List

SPEA2
=====

.. java:package:: org.uma.jmetal.algorithm.multiobjective.spea2
   :noindex:

.. java:type:: @SuppressWarnings public class SPEA2<S extends Solution<?>> extends AbstractGeneticAlgorithm<S, List<S>>

   :author: Juan J. Durillo

Fields
------
archive
^^^^^^^

.. java:field:: protected List<S> archive
   :outertype: SPEA2

environmentalSelection
^^^^^^^^^^^^^^^^^^^^^^

.. java:field:: protected final EnvironmentalSelection<S> environmentalSelection
   :outertype: SPEA2

evaluator
^^^^^^^^^

.. java:field:: protected final SolutionListEvaluator<S> evaluator
   :outertype: SPEA2

iterations
^^^^^^^^^^

.. java:field:: protected int iterations
   :outertype: SPEA2

maxIterations
^^^^^^^^^^^^^

.. java:field:: protected final int maxIterations
   :outertype: SPEA2

strenghtRawFitness
^^^^^^^^^^^^^^^^^^

.. java:field:: protected final StrengthRawFitness<S> strenghtRawFitness
   :outertype: SPEA2

Constructors
------------
SPEA2
^^^^^

.. java:constructor:: public SPEA2(Problem<S> problem, int maxIterations, int populationSize, CrossoverOperator<S> crossoverOperator, MutationOperator<S> mutationOperator, SelectionOperator<List<S>, S> selectionOperator, SolutionListEvaluator<S> evaluator)
   :outertype: SPEA2

Methods
-------
evaluatePopulation
^^^^^^^^^^^^^^^^^^

.. java:method:: @Override protected List<S> evaluatePopulation(List<S> population)
   :outertype: SPEA2

getDescription
^^^^^^^^^^^^^^

.. java:method:: @Override public String getDescription()
   :outertype: SPEA2

getName
^^^^^^^

.. java:method:: @Override public String getName()
   :outertype: SPEA2

getResult
^^^^^^^^^

.. java:method:: @Override public List<S> getResult()
   :outertype: SPEA2

initProgress
^^^^^^^^^^^^

.. java:method:: @Override protected void initProgress()
   :outertype: SPEA2

isStoppingConditionReached
^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override protected boolean isStoppingConditionReached()
   :outertype: SPEA2

replacement
^^^^^^^^^^^

.. java:method:: @Override protected List<S> replacement(List<S> population, List<S> offspringPopulation)
   :outertype: SPEA2

reproduction
^^^^^^^^^^^^

.. java:method:: @Override protected List<S> reproduction(List<S> population)
   :outertype: SPEA2

selection
^^^^^^^^^

.. java:method:: @Override protected List<S> selection(List<S> population)
   :outertype: SPEA2

updateProgress
^^^^^^^^^^^^^^

.. java:method:: @Override protected void updateProgress()
   :outertype: SPEA2

