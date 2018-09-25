.. java:import:: org.uma.jmetal.operator CrossoverOperator

.. java:import:: org.uma.jmetal.operator MutationOperator

.. java:import:: org.uma.jmetal.operator SelectionOperator

.. java:import:: org.uma.jmetal.problem Problem

.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util.evaluator SolutionListEvaluator

.. java:import:: java.util ArrayList

.. java:import:: java.util Collections

.. java:import:: java.util List

MOMBI2
======

.. java:package:: org.uma.jmetal.algorithm.multiobjective.mombi
   :noindex:

.. java:type:: @SuppressWarnings public class MOMBI2<S extends Solution<?>> extends MOMBI<S>

   :author: Juan J. Durillo

Fields
------
alpha
^^^^^

.. java:field:: protected final Double alpha
   :outertype: MOMBI2

epsilon
^^^^^^^

.. java:field:: protected final Double epsilon
   :outertype: MOMBI2

history
^^^^^^^

.. java:field:: protected final MOMBI2History<S> history
   :outertype: MOMBI2

maxs
^^^^

.. java:field:: protected List<Double> maxs
   :outertype: MOMBI2

normalizer
^^^^^^^^^^

.. java:field:: protected Normalizer normalizer
   :outertype: MOMBI2

Constructors
------------
MOMBI2
^^^^^^

.. java:constructor:: public MOMBI2(Problem<S> problem, int maxIterations, CrossoverOperator<S> crossover, MutationOperator<S> mutation, SelectionOperator<List<S>, S> selection, SolutionListEvaluator<S> evaluator, String pathWeights)
   :outertype: MOMBI2

   Creates a new instance of the MOMBI algorithm

   :param problem:
   :param maxIterations:
   :param crossover:
   :param mutation:
   :param selection:
   :param evaluator:
   :param pathWeights:

Methods
-------
computeRanking
^^^^^^^^^^^^^^

.. java:method:: protected R2Ranking<S> computeRanking(List<S> solutionList)
   :outertype: MOMBI2

createUtilityFunction
^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public AbstractUtilityFunctionsSet<S> createUtilityFunction(String pathWeights)
   :outertype: MOMBI2

getDescription
^^^^^^^^^^^^^^

.. java:method:: @Override public String getDescription()
   :outertype: MOMBI2

getMax
^^^^^^

.. java:method:: public Double getMax(List<Double> list)
   :outertype: MOMBI2

getName
^^^^^^^

.. java:method:: @Override public String getName()
   :outertype: MOMBI2

initProgress
^^^^^^^^^^^^

.. java:method:: @Override protected void initProgress()
   :outertype: MOMBI2

updateMax
^^^^^^^^^

.. java:method:: protected void updateMax(List<S> population)
   :outertype: MOMBI2

updateReferencePoint
^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public void updateReferencePoint(List<S> population)
   :outertype: MOMBI2

