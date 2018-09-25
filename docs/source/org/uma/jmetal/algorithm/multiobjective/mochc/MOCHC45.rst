.. java:import:: org.uma.jmetal.algorithm Algorithm

.. java:import:: org.uma.jmetal.algorithm.impl AbstractGeneticAlgorithm

.. java:import:: org.uma.jmetal.operator CrossoverOperator

.. java:import:: org.uma.jmetal.operator MutationOperator

.. java:import:: org.uma.jmetal.operator SelectionOperator

.. java:import:: org.uma.jmetal.problem BinaryProblem

.. java:import:: org.uma.jmetal.solution BinarySolution

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: org.uma.jmetal.util SolutionListUtils

.. java:import:: org.uma.jmetal.util.archive.impl NonDominatedSolutionListArchive

.. java:import:: org.uma.jmetal.util.binarySet BinarySet

.. java:import:: org.uma.jmetal.util.comparator CrowdingDistanceComparator

.. java:import:: org.uma.jmetal.util.evaluator SolutionListEvaluator

.. java:import:: java.util ArrayList

.. java:import:: java.util Collections

.. java:import:: java.util Comparator

.. java:import:: java.util List

MOCHC45
=======

.. java:package:: org.uma.jmetal.algorithm.multiobjective.mochc
   :noindex:

.. java:type:: @SuppressWarnings public class MOCHC45 implements Algorithm<List<BinarySolution>>

   This class executes the MOCHC algorithm described in: A.J. Nebro, E. Alba, G. Molina, F. Chicano, F. Luna, J.J. Durillo "Optimal antenna placement using a new multi-objective chc algorithm". GECCO '07: Proceedings of the 9th annual conference on Genetic and evolutionary computation. London, England. July 2007. Implementation of MOCHC following the scheme used in jMetal4.5 and former versions, i.e, without implementing the \ :java:ref:`AbstractGeneticAlgorithm`\  interface.

Constructors
------------
MOCHC45
^^^^^^^

.. java:constructor:: public MOCHC45(BinaryProblem problem, int populationSize, int maxEvaluations, int convergenceValue, double preservedPopulation, double initialConvergenceCount, CrossoverOperator<BinarySolution> crossoverOperator, MutationOperator<BinarySolution> cataclysmicMutation, SelectionOperator<List<BinarySolution>, List<BinarySolution>> newGenerationSelection, SelectionOperator<List<BinarySolution>, BinarySolution> parentSelection, SolutionListEvaluator<BinarySolution> evaluator)
   :outertype: MOCHC45

   Constructor

Methods
-------
getDescription
^^^^^^^^^^^^^^

.. java:method:: @Override public String getDescription()
   :outertype: MOCHC45

getName
^^^^^^^

.. java:method:: @Override public String getName()
   :outertype: MOCHC45

getResult
^^^^^^^^^

.. java:method:: @Override public List<BinarySolution> getResult()
   :outertype: MOCHC45

run
^^^

.. java:method:: @Override public void run()
   :outertype: MOCHC45

