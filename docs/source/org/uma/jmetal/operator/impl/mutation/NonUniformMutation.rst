.. java:import:: org.uma.jmetal.operator MutationOperator

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: org.uma.jmetal.util.pseudorandom JMetalRandom

.. java:import:: org.uma.jmetal.util.pseudorandom RandomGenerator

NonUniformMutation
==================

.. java:package:: org.uma.jmetal.operator.impl.mutation
   :noindex:

.. java:type:: @SuppressWarnings public class NonUniformMutation implements MutationOperator<DoubleSolution>

   This class implements a non-uniform mutation operator.

   :author: Antonio J. Nebro , Juan J. Durillo

Constructors
------------
NonUniformMutation
^^^^^^^^^^^^^^^^^^

.. java:constructor:: public NonUniformMutation(double mutationProbability, double perturbation, int maxIterations)
   :outertype: NonUniformMutation

   Constructor

NonUniformMutation
^^^^^^^^^^^^^^^^^^

.. java:constructor:: public NonUniformMutation(double mutationProbability, double perturbation, int maxIterations, RandomGenerator<Double> randomGenenerator)
   :outertype: NonUniformMutation

   Constructor

Methods
-------
doMutation
^^^^^^^^^^

.. java:method:: public void doMutation(double probability, DoubleSolution solution)
   :outertype: NonUniformMutation

   Perform the mutation operation

   :param probability: Mutation setProbability
   :param solution: The solution to mutate

execute
^^^^^^^

.. java:method:: @Override public DoubleSolution execute(DoubleSolution solution)
   :outertype: NonUniformMutation

   Execute() method

getCurrentIteration
^^^^^^^^^^^^^^^^^^^

.. java:method:: public int getCurrentIteration()
   :outertype: NonUniformMutation

getMaxIterations
^^^^^^^^^^^^^^^^

.. java:method:: public int getMaxIterations()
   :outertype: NonUniformMutation

getMutationProbability
^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public double getMutationProbability()
   :outertype: NonUniformMutation

getPerturbation
^^^^^^^^^^^^^^^

.. java:method:: public double getPerturbation()
   :outertype: NonUniformMutation

setCurrentIteration
^^^^^^^^^^^^^^^^^^^

.. java:method:: public void setCurrentIteration(int currentIteration)
   :outertype: NonUniformMutation

setMaxIterations
^^^^^^^^^^^^^^^^

.. java:method:: public void setMaxIterations(int maxIterations)
   :outertype: NonUniformMutation

setMutationProbability
^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public void setMutationProbability(double mutationProbability)
   :outertype: NonUniformMutation

setPerturbation
^^^^^^^^^^^^^^^

.. java:method:: public void setPerturbation(double perturbation)
   :outertype: NonUniformMutation

