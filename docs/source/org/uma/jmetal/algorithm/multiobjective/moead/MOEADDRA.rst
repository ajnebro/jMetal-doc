.. java:import:: org.uma.jmetal.algorithm.multiobjective.moead.util MOEADUtils

.. java:import:: org.uma.jmetal.operator CrossoverOperator

.. java:import:: org.uma.jmetal.operator MutationOperator

.. java:import:: org.uma.jmetal.operator.impl.crossover DifferentialEvolutionCrossover

.. java:import:: org.uma.jmetal.problem Problem

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: org.uma.jmetal.util.pseudorandom JMetalRandom

.. java:import:: java.util ArrayList

.. java:import:: java.util List

MOEADDRA
========

.. java:package:: org.uma.jmetal.algorithm.multiobjective.moead
   :noindex:

.. java:type:: @SuppressWarnings public class MOEADDRA extends AbstractMOEAD<DoubleSolution>

   Class implementing the MOEA/D-DRA algorithm described in : Q. Zhang, W. Liu, and H Li, The Performance of a New Version of MOEA/D on CEC09 Unconstrained MOP Test Instances, Working Report CES-491, School of CS & EE, University of Essex, 02/2009

   :author: Juan J. Durillo, Antonio J. Nebro

Fields
------
differentialEvolutionCrossover
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:field:: protected DifferentialEvolutionCrossover differentialEvolutionCrossover
   :outertype: MOEADDRA

frequency
^^^^^^^^^

.. java:field:: protected int[] frequency
   :outertype: MOEADDRA

randomGenerator
^^^^^^^^^^^^^^^

.. java:field::  JMetalRandom randomGenerator
   :outertype: MOEADDRA

savedValues
^^^^^^^^^^^

.. java:field:: protected DoubleSolution[] savedValues
   :outertype: MOEADDRA

utility
^^^^^^^

.. java:field:: protected double[] utility
   :outertype: MOEADDRA

Constructors
------------
MOEADDRA
^^^^^^^^

.. java:constructor:: public MOEADDRA(Problem<DoubleSolution> problem, int populationSize, int resultPopulationSize, int maxEvaluations, MutationOperator<DoubleSolution> mutation, CrossoverOperator<DoubleSolution> crossover, FunctionType functionType, String dataDirectory, double neighborhoodSelectionProbability, int maximumNumberOfReplacedSolutions, int neighborSize)
   :outertype: MOEADDRA

Methods
-------
getDescription
^^^^^^^^^^^^^^

.. java:method:: @Override public String getDescription()
   :outertype: MOEADDRA

getName
^^^^^^^

.. java:method:: @Override public String getName()
   :outertype: MOEADDRA

initializePopulation
^^^^^^^^^^^^^^^^^^^^

.. java:method:: protected void initializePopulation()
   :outertype: MOEADDRA

run
^^^

.. java:method:: @Override public void run()
   :outertype: MOEADDRA

tourSelection
^^^^^^^^^^^^^

.. java:method:: public List<Integer> tourSelection(int depth)
   :outertype: MOEADDRA

utilityFunction
^^^^^^^^^^^^^^^

.. java:method:: public void utilityFunction() throws JMetalException
   :outertype: MOEADDRA

