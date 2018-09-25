.. java:import:: org.uma.jmetal.operator MutationOperator

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: org.uma.jmetal.util.pseudorandom JMetalRandom

.. java:import:: org.uma.jmetal.util.pseudorandom RandomGenerator

UniformMutation
===============

.. java:package:: org.uma.jmetal.operator.impl.mutation
   :noindex:

.. java:type:: @SuppressWarnings public class UniformMutation implements MutationOperator<DoubleSolution>

   This class implements a uniform mutation operator.

   :author: Antonio J. Nebro , Juan J. Durillo

Constructors
------------
UniformMutation
^^^^^^^^^^^^^^^

.. java:constructor:: public UniformMutation(double mutationProbability, double perturbation)
   :outertype: UniformMutation

   Constructor

UniformMutation
^^^^^^^^^^^^^^^

.. java:constructor:: public UniformMutation(double mutationProbability, double perturbation, RandomGenerator<Double> randomGenenerator)
   :outertype: UniformMutation

   Constructor

Methods
-------
doMutation
^^^^^^^^^^

.. java:method:: public void doMutation(double probability, DoubleSolution solution)
   :outertype: UniformMutation

   Perform the operation

   :param probability: Mutation setProbability
   :param solution: The solution to mutate

execute
^^^^^^^

.. java:method:: @Override public DoubleSolution execute(DoubleSolution solution)
   :outertype: UniformMutation

   Execute() method

getMutationProbability
^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public Double getMutationProbability()
   :outertype: UniformMutation

getPerturbation
^^^^^^^^^^^^^^^

.. java:method:: public double getPerturbation()
   :outertype: UniformMutation

setMutationProbability
^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public void setMutationProbability(Double mutationProbability)
   :outertype: UniformMutation

setPerturbation
^^^^^^^^^^^^^^^

.. java:method:: public void setPerturbation(Double perturbation)
   :outertype: UniformMutation

