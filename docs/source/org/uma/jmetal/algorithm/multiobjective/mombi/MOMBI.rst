.. java:import:: org.uma.jmetal.operator CrossoverOperator

.. java:import:: org.uma.jmetal.operator MutationOperator

.. java:import:: org.uma.jmetal.operator SelectionOperator

.. java:import:: org.uma.jmetal.problem Problem

.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util.evaluator SolutionListEvaluator

.. java:import:: java.util ArrayList

.. java:import:: java.util Collections

.. java:import:: java.util Comparator

.. java:import:: java.util List

MOMBI
=====

.. java:package:: org.uma.jmetal.algorithm.multiobjective.mombi
   :noindex:

.. java:type:: @SuppressWarnings public class MOMBI<S extends Solution<?>> extends AbstractMOMBI<S>

Fields
------
utilityFunctions
^^^^^^^^^^^^^^^^

.. java:field:: protected final AbstractUtilityFunctionsSet<S> utilityFunctions
   :outertype: MOMBI

Constructors
------------
MOMBI
^^^^^

.. java:constructor:: public MOMBI(Problem<S> problem, int maxIterations, CrossoverOperator<S> crossover, MutationOperator<S> mutation, SelectionOperator<List<S>, S> selection, SolutionListEvaluator<S> evaluator, String pathWeights)
   :outertype: MOMBI

Methods
-------
addLastRankedSolutionsToPopulation
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: protected void addLastRankedSolutionsToPopulation(R2Ranking<S> ranking, int index, List<S> population)
   :outertype: MOMBI

addRankedSolutionsToPopulation
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: protected void addRankedSolutionsToPopulation(R2Ranking<S> ranking, int index, List<S> population)
   :outertype: MOMBI

computeRanking
^^^^^^^^^^^^^^

.. java:method:: protected R2Ranking<S> computeRanking(List<S> solutionList)
   :outertype: MOMBI

createUtilityFunction
^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public AbstractUtilityFunctionsSet<S> createUtilityFunction(String pathWeights)
   :outertype: MOMBI

getDescription
^^^^^^^^^^^^^^

.. java:method:: @Override public String getDescription()
   :outertype: MOMBI

getMaxPopulationSize
^^^^^^^^^^^^^^^^^^^^

.. java:method:: public int getMaxPopulationSize()
   :outertype: MOMBI

getName
^^^^^^^

.. java:method:: @Override public String getName()
   :outertype: MOMBI

getUtilityFunctions
^^^^^^^^^^^^^^^^^^^

.. java:method:: protected AbstractUtilityFunctionsSet<S> getUtilityFunctions()
   :outertype: MOMBI

replacement
^^^^^^^^^^^

.. java:method:: @Override protected List<S> replacement(List<S> population, List<S> offspringPopulation)
   :outertype: MOMBI

selectBest
^^^^^^^^^^

.. java:method:: protected List<S> selectBest(R2Ranking<S> ranking)
   :outertype: MOMBI

specificMOEAComputations
^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public void specificMOEAComputations()
   :outertype: MOMBI

