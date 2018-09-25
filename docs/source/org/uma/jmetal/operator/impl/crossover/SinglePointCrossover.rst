.. java:import:: org.uma.jmetal.operator CrossoverOperator

.. java:import:: org.uma.jmetal.solution BinarySolution

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: org.uma.jmetal.util.binarySet BinarySet

.. java:import:: org.uma.jmetal.util.pseudorandom BoundedRandomGenerator

.. java:import:: org.uma.jmetal.util.pseudorandom JMetalRandom

.. java:import:: org.uma.jmetal.util.pseudorandom RandomGenerator

.. java:import:: java.util ArrayList

.. java:import:: java.util List

SinglePointCrossover
====================

.. java:package:: org.uma.jmetal.operator.impl.crossover
   :noindex:

.. java:type:: @SuppressWarnings public class SinglePointCrossover implements CrossoverOperator<BinarySolution>

   This class implements a single point crossover operator.

   :author: Antonio J. Nebro

Constructors
------------
SinglePointCrossover
^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public SinglePointCrossover(double crossoverProbability)
   :outertype: SinglePointCrossover

   Constructor

SinglePointCrossover
^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public SinglePointCrossover(double crossoverProbability, RandomGenerator<Double> randomGenerator)
   :outertype: SinglePointCrossover

   Constructor

SinglePointCrossover
^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public SinglePointCrossover(double crossoverProbability, RandomGenerator<Double> crossoverRandomGenerator, BoundedRandomGenerator<Integer> pointRandomGenerator)
   :outertype: SinglePointCrossover

   Constructor

Methods
-------
doCrossover
^^^^^^^^^^^

.. java:method:: public List<BinarySolution> doCrossover(double probability, BinarySolution parent1, BinarySolution parent2)
   :outertype: SinglePointCrossover

   Perform the crossover operation.

   :param probability: Crossover setProbability
   :param parent1: The first parent
   :param parent2: The second parent
   :return: An array containing the two offspring

execute
^^^^^^^

.. java:method:: @Override public List<BinarySolution> execute(List<BinarySolution> solutions)
   :outertype: SinglePointCrossover

getCrossoverProbability
^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public double getCrossoverProbability()
   :outertype: SinglePointCrossover

getNumberOfGeneratedChildren
^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public int getNumberOfGeneratedChildren()
   :outertype: SinglePointCrossover

getNumberOfRequiredParents
^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public int getNumberOfRequiredParents()
   :outertype: SinglePointCrossover

setCrossoverProbability
^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public void setCrossoverProbability(double crossoverProbability)
   :outertype: SinglePointCrossover

