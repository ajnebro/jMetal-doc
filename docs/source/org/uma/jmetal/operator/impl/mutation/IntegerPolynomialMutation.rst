.. java:import:: org.uma.jmetal.operator MutationOperator

.. java:import:: org.uma.jmetal.problem IntegerProblem

.. java:import:: org.uma.jmetal.solution IntegerSolution

.. java:import:: org.uma.jmetal.solution.util RepairDoubleSolution

.. java:import:: org.uma.jmetal.solution.util RepairDoubleSolutionAtBounds

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: org.uma.jmetal.util.pseudorandom JMetalRandom

.. java:import:: org.uma.jmetal.util.pseudorandom RandomGenerator

IntegerPolynomialMutation
=========================

.. java:package:: org.uma.jmetal.operator.impl.mutation
   :noindex:

.. java:type:: @SuppressWarnings public class IntegerPolynomialMutation implements MutationOperator<IntegerSolution>

   This class implements a polynomial mutation operator to be applied to Integer solutions If the lower and upper bounds of a variable are the same, no mutation is carried out and the bound value is returned. A \ :java:ref:`RepairDoubleSolution`\  object is used to decide the strategy to apply when a value is out of range.

   :author: Antonio J. Nebro

Constructors
------------
IntegerPolynomialMutation
^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public IntegerPolynomialMutation()
   :outertype: IntegerPolynomialMutation

   Constructor

IntegerPolynomialMutation
^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public IntegerPolynomialMutation(IntegerProblem problem, double distributionIndex)
   :outertype: IntegerPolynomialMutation

   Constructor

IntegerPolynomialMutation
^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public IntegerPolynomialMutation(double mutationProbability, double distributionIndex)
   :outertype: IntegerPolynomialMutation

   Constructor

IntegerPolynomialMutation
^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public IntegerPolynomialMutation(double mutationProbability, double distributionIndex, RepairDoubleSolution solutionRepair)
   :outertype: IntegerPolynomialMutation

   Constructor

IntegerPolynomialMutation
^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public IntegerPolynomialMutation(double mutationProbability, double distributionIndex, RepairDoubleSolution solutionRepair, RandomGenerator<Double> randomGenerator)
   :outertype: IntegerPolynomialMutation

   Constructor

Methods
-------
execute
^^^^^^^

.. java:method:: public IntegerSolution execute(IntegerSolution solution) throws JMetalException
   :outertype: IntegerPolynomialMutation

   Execute() method

getDistributionIndex
^^^^^^^^^^^^^^^^^^^^

.. java:method:: public double getDistributionIndex()
   :outertype: IntegerPolynomialMutation

getMutationProbability
^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public double getMutationProbability()
   :outertype: IntegerPolynomialMutation

setDistributionIndex
^^^^^^^^^^^^^^^^^^^^

.. java:method:: public void setDistributionIndex(double distributionIndex)
   :outertype: IntegerPolynomialMutation

setMutationProbability
^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public void setMutationProbability(double mutationProbability)
   :outertype: IntegerPolynomialMutation

