.. java:import:: org.uma.jmetal.operator CrossoverOperator

.. java:import:: org.uma.jmetal.solution PermutationSolution

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: org.uma.jmetal.util.pseudorandom BoundedRandomGenerator

.. java:import:: org.uma.jmetal.util.pseudorandom JMetalRandom

.. java:import:: org.uma.jmetal.util.pseudorandom RandomGenerator

.. java:import:: java.util ArrayList

.. java:import:: java.util List

PMXCrossover
============

.. java:package:: org.uma.jmetal.operator.impl.crossover
   :noindex:

.. java:type:: @SuppressWarnings public class PMXCrossover implements CrossoverOperator<PermutationSolution<Integer>>

   This class allows to apply a PMX crossover operator using two parent solutions.

   :author: Antonio J. Nebro , Juan J. Durillo

Constructors
------------
PMXCrossover
^^^^^^^^^^^^

.. java:constructor:: public PMXCrossover(double crossoverProbability)
   :outertype: PMXCrossover

   Constructor

PMXCrossover
^^^^^^^^^^^^

.. java:constructor:: public PMXCrossover(double crossoverProbability, RandomGenerator<Double> randomGenerator)
   :outertype: PMXCrossover

   Constructor

PMXCrossover
^^^^^^^^^^^^

.. java:constructor:: public PMXCrossover(double crossoverProbability, RandomGenerator<Double> crossoverRandomGenerator, BoundedRandomGenerator<Integer> cuttingPointRandomGenerator)
   :outertype: PMXCrossover

   Constructor

Methods
-------
doCrossover
^^^^^^^^^^^

.. java:method:: public List<PermutationSolution<Integer>> doCrossover(double probability, List<PermutationSolution<Integer>> parents)
   :outertype: PMXCrossover

   Perform the crossover operation

   :param probability: Crossover probability
   :param parents: Parents
   :return: An array containing the two offspring

execute
^^^^^^^

.. java:method:: public List<PermutationSolution<Integer>> execute(List<PermutationSolution<Integer>> parents)
   :outertype: PMXCrossover

   Executes the operation

   :param parents: An object containing an array of two solutions

getCrossoverProbability
^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public double getCrossoverProbability()
   :outertype: PMXCrossover

getNumberOfGeneratedChildren
^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public int getNumberOfGeneratedChildren()
   :outertype: PMXCrossover

getNumberOfRequiredParents
^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public int getNumberOfRequiredParents()
   :outertype: PMXCrossover

setCrossoverProbability
^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public void setCrossoverProbability(double crossoverProbability)
   :outertype: PMXCrossover

