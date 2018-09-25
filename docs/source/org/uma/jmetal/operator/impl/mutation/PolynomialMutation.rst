.. java:import:: org.uma.jmetal.operator MutationOperator

.. java:import:: org.uma.jmetal.problem DoubleProblem

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.solution.util RepairDoubleSolution

.. java:import:: org.uma.jmetal.solution.util RepairDoubleSolutionAtBounds

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: org.uma.jmetal.util.pseudorandom JMetalRandom

.. java:import:: org.uma.jmetal.util.pseudorandom RandomGenerator

PolynomialMutation
==================

.. java:package:: org.uma.jmetal.operator.impl.mutation
   :noindex:

.. java:type:: @SuppressWarnings public class PolynomialMutation implements MutationOperator<DoubleSolution>

   This class implements a polynomial mutation operator The implementation is based on the NSGA-II code available in http://www.iitk.ac.in/kangal/codes.shtml If the lower and upper bounds of a variable are the same, no mutation is carried out and the bound value is returned.

   :author: Antonio J. Nebro , Juan J. Durillo

Constructors
------------
PolynomialMutation
^^^^^^^^^^^^^^^^^^

.. java:constructor:: public PolynomialMutation()
   :outertype: PolynomialMutation

   Constructor

PolynomialMutation
^^^^^^^^^^^^^^^^^^

.. java:constructor:: public PolynomialMutation(DoubleProblem problem, double distributionIndex)
   :outertype: PolynomialMutation

   Constructor

PolynomialMutation
^^^^^^^^^^^^^^^^^^

.. java:constructor:: public PolynomialMutation(DoubleProblem problem, double distributionIndex, RandomGenerator<Double> randomGenerator)
   :outertype: PolynomialMutation

   Constructor

PolynomialMutation
^^^^^^^^^^^^^^^^^^

.. java:constructor:: public PolynomialMutation(double mutationProbability, double distributionIndex)
   :outertype: PolynomialMutation

   Constructor

PolynomialMutation
^^^^^^^^^^^^^^^^^^

.. java:constructor:: public PolynomialMutation(double mutationProbability, double distributionIndex, RandomGenerator<Double> randomGenerator)
   :outertype: PolynomialMutation

   Constructor

PolynomialMutation
^^^^^^^^^^^^^^^^^^

.. java:constructor:: public PolynomialMutation(double mutationProbability, double distributionIndex, RepairDoubleSolution solutionRepair)
   :outertype: PolynomialMutation

   Constructor

PolynomialMutation
^^^^^^^^^^^^^^^^^^

.. java:constructor:: public PolynomialMutation(double mutationProbability, double distributionIndex, RepairDoubleSolution solutionRepair, RandomGenerator<Double> randomGenerator)
   :outertype: PolynomialMutation

   Constructor

Methods
-------
execute
^^^^^^^

.. java:method:: @Override public DoubleSolution execute(DoubleSolution solution) throws JMetalException
   :outertype: PolynomialMutation

   Execute() method

getDistributionIndex
^^^^^^^^^^^^^^^^^^^^

.. java:method:: public double getDistributionIndex()
   :outertype: PolynomialMutation

getMutationProbability
^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public double getMutationProbability()
   :outertype: PolynomialMutation

setDistributionIndex
^^^^^^^^^^^^^^^^^^^^

.. java:method:: public void setDistributionIndex(double distributionIndex)
   :outertype: PolynomialMutation

setMutationProbability
^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public void setMutationProbability(double probability)
   :outertype: PolynomialMutation

