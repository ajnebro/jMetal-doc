.. java:import:: org.uma.jmetal.operator MutationOperator

.. java:import:: org.uma.jmetal.solution PermutationSolution

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: org.uma.jmetal.util.pseudorandom BoundedRandomGenerator

.. java:import:: org.uma.jmetal.util.pseudorandom JMetalRandom

.. java:import:: org.uma.jmetal.util.pseudorandom RandomGenerator

PermutationSwapMutation
=======================

.. java:package:: org.uma.jmetal.operator.impl.mutation
   :noindex:

.. java:type:: @SuppressWarnings public class PermutationSwapMutation<T> implements MutationOperator<PermutationSolution<T>>

   This class implements a swap mutation. The solution type of the solution must be Permutation.

   :author: Antonio J. Nebro , Juan J. Durillo

Constructors
------------
PermutationSwapMutation
^^^^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public PermutationSwapMutation(double mutationProbability)
   :outertype: PermutationSwapMutation

   Constructor

PermutationSwapMutation
^^^^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public PermutationSwapMutation(double mutationProbability, RandomGenerator<Double> randomGenerator)
   :outertype: PermutationSwapMutation

   Constructor

PermutationSwapMutation
^^^^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public PermutationSwapMutation(double mutationProbability, RandomGenerator<Double> mutationRandomGenerator, BoundedRandomGenerator<Integer> positionRandomGenerator)
   :outertype: PermutationSwapMutation

   Constructor

Methods
-------
doMutation
^^^^^^^^^^

.. java:method:: public void doMutation(PermutationSolution<T> solution)
   :outertype: PermutationSwapMutation

   Performs the operation

execute
^^^^^^^

.. java:method:: @Override public PermutationSolution<T> execute(PermutationSolution<T> solution)
   :outertype: PermutationSwapMutation

getMutationProbability
^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public double getMutationProbability()
   :outertype: PermutationSwapMutation

setMutationProbability
^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public void setMutationProbability(double mutationProbability)
   :outertype: PermutationSwapMutation

