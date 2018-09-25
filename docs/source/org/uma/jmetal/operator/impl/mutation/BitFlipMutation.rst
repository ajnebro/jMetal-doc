.. java:import:: org.uma.jmetal.operator MutationOperator

.. java:import:: org.uma.jmetal.solution BinarySolution

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: org.uma.jmetal.util.pseudorandom JMetalRandom

.. java:import:: org.uma.jmetal.util.pseudorandom RandomGenerator

BitFlipMutation
===============

.. java:package:: org.uma.jmetal.operator.impl.mutation
   :noindex:

.. java:type:: @SuppressWarnings public class BitFlipMutation implements MutationOperator<BinarySolution>

   :author: Antonio J. Nebro

Constructors
------------
BitFlipMutation
^^^^^^^^^^^^^^^

.. java:constructor:: public BitFlipMutation(double mutationProbability)
   :outertype: BitFlipMutation

   Constructor

BitFlipMutation
^^^^^^^^^^^^^^^

.. java:constructor:: public BitFlipMutation(double mutationProbability, RandomGenerator<Double> randomGenerator)
   :outertype: BitFlipMutation

   Constructor

Methods
-------
doMutation
^^^^^^^^^^

.. java:method:: public void doMutation(double probability, BinarySolution solution)
   :outertype: BitFlipMutation

   Perform the mutation operation

   :param probability: Mutation setProbability
   :param solution: The solution to mutate

execute
^^^^^^^

.. java:method:: @Override public BinarySolution execute(BinarySolution solution)
   :outertype: BitFlipMutation

   Execute() method

getMutationProbability
^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public double getMutationProbability()
   :outertype: BitFlipMutation

setMutationProbability
^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public void setMutationProbability(double mutationProbability)
   :outertype: BitFlipMutation

