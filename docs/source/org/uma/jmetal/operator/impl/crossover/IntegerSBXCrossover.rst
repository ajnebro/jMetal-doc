.. java:import:: org.uma.jmetal.operator CrossoverOperator

.. java:import:: org.uma.jmetal.solution IntegerSolution

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: org.uma.jmetal.util.pseudorandom JMetalRandom

.. java:import:: org.uma.jmetal.util.pseudorandom RandomGenerator

.. java:import:: java.util ArrayList

.. java:import:: java.util List

IntegerSBXCrossover
===================

.. java:package:: org.uma.jmetal.operator.impl.crossover
   :noindex:

.. java:type:: @SuppressWarnings public class IntegerSBXCrossover implements CrossoverOperator<IntegerSolution>

   This class allows to apply a SBX crossover operator using two parent solutions (Integer encoding)

   :author: Antonio J. Nebro

Constructors
------------
IntegerSBXCrossover
^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public IntegerSBXCrossover(double crossoverProbability, double distributionIndex)
   :outertype: IntegerSBXCrossover

   Constructor

IntegerSBXCrossover
^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public IntegerSBXCrossover(double crossoverProbability, double distributionIndex, RandomGenerator<Double> randomGenerator)
   :outertype: IntegerSBXCrossover

   Constructor

Methods
-------
doCrossover
^^^^^^^^^^^

.. java:method:: public List<IntegerSolution> doCrossover(double probability, IntegerSolution parent1, IntegerSolution parent2)
   :outertype: IntegerSBXCrossover

   doCrossover method

execute
^^^^^^^

.. java:method:: @Override public List<IntegerSolution> execute(List<IntegerSolution> solutions)
   :outertype: IntegerSBXCrossover

   Execute() method

getCrossoverProbability
^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public double getCrossoverProbability()
   :outertype: IntegerSBXCrossover

getDistributionIndex
^^^^^^^^^^^^^^^^^^^^

.. java:method:: public double getDistributionIndex()
   :outertype: IntegerSBXCrossover

getNumberOfGeneratedChildren
^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public int getNumberOfGeneratedChildren()
   :outertype: IntegerSBXCrossover

getNumberOfRequiredParents
^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public int getNumberOfRequiredParents()
   :outertype: IntegerSBXCrossover

setCrossoverProbability
^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public void setCrossoverProbability(double crossoverProbability)
   :outertype: IntegerSBXCrossover

setDistributionIndex
^^^^^^^^^^^^^^^^^^^^

.. java:method:: public void setDistributionIndex(double distributionIndex)
   :outertype: IntegerSBXCrossover

