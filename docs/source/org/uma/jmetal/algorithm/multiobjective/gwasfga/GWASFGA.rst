.. java:import:: org.uma.jmetal.algorithm.multiobjective.gwasfga.util GWASFGARanking

.. java:import:: org.uma.jmetal.algorithm.multiobjective.mombi.util ASFWASFGA

.. java:import:: org.uma.jmetal.algorithm.multiobjective.mombi.util AbstractUtilityFunctionsSet

.. java:import:: org.uma.jmetal.algorithm.multiobjective.wasfga WASFGA

.. java:import:: org.uma.jmetal.operator CrossoverOperator

.. java:import:: org.uma.jmetal.operator MutationOperator

.. java:import:: org.uma.jmetal.operator SelectionOperator

.. java:import:: org.uma.jmetal.problem Problem

.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util.evaluator SolutionListEvaluator

.. java:import:: org.uma.jmetal.util.solutionattribute Ranking

.. java:import:: java.util List

GWASFGA
=======

.. java:package:: org.uma.jmetal.algorithm.multiobjective.gwasfga
   :noindex:

.. java:type:: public class GWASFGA<S extends Solution<?>> extends WASFGA<S>

   This class executes the GWASFGA algorithm described in: Saborido, R., Ruiz, A. B. and Luque, M. (2015). Global WASF-GA: An Evolutionary Algorithm in Multiobjective Optimization to Approximate the whole Pareto Optimal Front. Evolutionary Computation Accepted for publication.

   :author: Juanjo Durillo

Constructors
------------
GWASFGA
^^^^^^^

.. java:constructor:: public GWASFGA(Problem<S> problem, int populationSize, int maxIterations, CrossoverOperator<S> crossoverOperator, MutationOperator<S> mutationOperator, SelectionOperator<List<S>, S> selectionOperator, SolutionListEvaluator<S> evaluator, double epsilon, String weightVectorsFileName)
   :outertype: GWASFGA

GWASFGA
^^^^^^^

.. java:constructor:: public GWASFGA(Problem<S> problem, int populationSize, int maxIterations, CrossoverOperator<S> crossoverOperator, MutationOperator<S> mutationOperator, SelectionOperator<List<S>, S> selectionOperator, SolutionListEvaluator<S> evaluator, double epsilon)
   :outertype: GWASFGA

Methods
-------
computeRanking
^^^^^^^^^^^^^^

.. java:method:: protected Ranking<S> computeRanking(List<S> solutionList)
   :outertype: GWASFGA

getDescription
^^^^^^^^^^^^^^

.. java:method:: @Override public String getDescription()
   :outertype: GWASFGA

getName
^^^^^^^

.. java:method:: @Override public String getName()
   :outertype: GWASFGA

