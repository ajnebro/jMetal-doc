.. java:import:: org.uma.jmetal.operator CrossoverOperator

.. java:import:: org.uma.jmetal.solution BinarySolution

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: org.uma.jmetal.util.binarySet BinarySet

.. java:import:: org.uma.jmetal.util.pseudorandom JMetalRandom

.. java:import:: org.uma.jmetal.util.pseudorandom RandomGenerator

.. java:import:: java.util ArrayList

.. java:import:: java.util List

HUXCrossover
============

.. java:package:: org.uma.jmetal.operator.impl.crossover
   :noindex:

.. java:type:: @SuppressWarnings public class HUXCrossover implements CrossoverOperator<BinarySolution>

   This class allows to apply a HUX crossover operator using two parent solutions. NOTE: the operator is applied to the first encoding.variable of the solutions, and the type of the solutions must be Binary

   :author: Antonio J. Nebro, Juan J. Durillo

Constructors
------------
HUXCrossover
^^^^^^^^^^^^

.. java:constructor:: public HUXCrossover(double crossoverProbability)
   :outertype: HUXCrossover

   Constructor

HUXCrossover
^^^^^^^^^^^^

.. java:constructor:: public HUXCrossover(double crossoverProbability, RandomGenerator<Double> randomGenerator)
   :outertype: HUXCrossover

   Constructor

Methods
-------
doCrossover
^^^^^^^^^^^

.. java:method:: public List<BinarySolution> doCrossover(double probability, BinarySolution parent1, BinarySolution parent2) throws JMetalException
   :outertype: HUXCrossover

   Perform the crossover operation

   :param probability: Crossover setProbability
   :param parent1: The first parent
   :param parent2: The second parent
   :throws org.uma.jmetal.util.JMetalException:
   :return: An array containing the two offspring

execute
^^^^^^^

.. java:method:: public List<BinarySolution> execute(List<BinarySolution> parents)
   :outertype: HUXCrossover

   Execute() method

getCrossoverProbability
^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public double getCrossoverProbability()
   :outertype: HUXCrossover

getNumberOfGeneratedChildren
^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public int getNumberOfGeneratedChildren()
   :outertype: HUXCrossover

getNumberOfRequiredParents
^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public int getNumberOfRequiredParents()
   :outertype: HUXCrossover

setCrossoverProbability
^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public void setCrossoverProbability(double crossoverProbability)
   :outertype: HUXCrossover

