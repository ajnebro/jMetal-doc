.. java:import:: org.uma.jmetal.operator MutationOperator

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: org.uma.jmetal.util.pseudorandom JMetalRandom

.. java:import:: org.uma.jmetal.util.pseudorandom RandomGenerator

SimpleRandomMutation
====================

.. java:package:: org.uma.jmetal.operator.impl.mutation
   :noindex:

.. java:type:: @SuppressWarnings public class SimpleRandomMutation implements MutationOperator<DoubleSolution>

   This class implements a random mutation operator for double solutions

   :author: Antonio J. Nebro

Constructors
------------
SimpleRandomMutation
^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public SimpleRandomMutation(double probability)
   :outertype: SimpleRandomMutation

   Constructor

SimpleRandomMutation
^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public SimpleRandomMutation(double probability, RandomGenerator<Double> randomGenerator)
   :outertype: SimpleRandomMutation

   Constructor

Methods
-------
execute
^^^^^^^

.. java:method:: @Override public DoubleSolution execute(DoubleSolution solution) throws JMetalException
   :outertype: SimpleRandomMutation

   Execute() method

getMutationProbability
^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public double getMutationProbability()
   :outertype: SimpleRandomMutation

setMutationProbability
^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public void setMutationProbability(double mutationProbability)
   :outertype: SimpleRandomMutation

