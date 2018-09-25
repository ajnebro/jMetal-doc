.. java:import:: org.hamcrest Matchers

.. java:import:: org.junit Test

.. java:import:: org.mockito Mockito

.. java:import:: org.springframework.test.util ReflectionTestUtils

.. java:import:: org.uma.jmetal.problem DoubleProblem

.. java:import:: org.uma.jmetal.problem.impl AbstractDoubleProblem

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.solution.impl DefaultDoubleSolution

.. java:import:: org.uma.jmetal.solution.util RepairDoubleSolutionAtBounds

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: org.uma.jmetal.util.pseudorandom JMetalRandom

.. java:import:: org.uma.jmetal.util.pseudorandom RandomGenerator

.. java:import:: org.uma.jmetal.util.pseudorandom.impl AuditableRandomGenerator

.. java:import:: java.util ArrayList

.. java:import:: java.util Arrays

.. java:import:: java.util List

.. java:import:: java.util Random

PolynomialMutationTest
======================

.. java:package:: org.uma.jmetal.operator.impl.mutation
   :noindex:

.. java:type:: public class PolynomialMutationTest

   Note: this class does check that the polynomial mutation operator does not return invalid values, but not that it works properly (@see PolynomialMutationWorkingTest)

   :author: Antonio J. Nebro

Methods
-------
shouldConstructorAssignTheCorrectDistributionIndex
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldConstructorAssignTheCorrectDistributionIndex()
   :outertype: PolynomialMutationTest

shouldConstructorAssignTheCorrectProbabilityValue
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldConstructorAssignTheCorrectProbabilityValue()
   :outertype: PolynomialMutationTest

shouldConstructorFailWhenPassedANegativeDistributionIndex
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldConstructorFailWhenPassedANegativeDistributionIndex()
   :outertype: PolynomialMutationTest

shouldConstructorFailWhenPassedANegativeProbabilityValue
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldConstructorFailWhenPassedANegativeProbabilityValue()
   :outertype: PolynomialMutationTest

shouldConstructorWithProblemAndDistributionIndexParametersAssignTheCorrectValues
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldConstructorWithProblemAndDistributionIndexParametersAssignTheCorrectValues()
   :outertype: PolynomialMutationTest

shouldConstructorWithoutParameterAssignTheDefaultValues
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldConstructorWithoutParameterAssignTheDefaultValues()
   :outertype: PolynomialMutationTest

shouldExecuteWithNullParameterThrowAnException
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldExecuteWithNullParameterThrowAnException()
   :outertype: PolynomialMutationTest

shouldGetDistributionIndexReturnTheRightValue
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldGetDistributionIndexReturnTheRightValue()
   :outertype: PolynomialMutationTest

shouldGetMutationProbabilityReturnTheRightValue
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldGetMutationProbabilityReturnTheRightValue()
   :outertype: PolynomialMutationTest

shouldJMetalRandomGeneratorNotBeUsedWhenCustomRandomGeneratorProvided
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldJMetalRandomGeneratorNotBeUsedWhenCustomRandomGeneratorProvided()
   :outertype: PolynomialMutationTest

shouldMutateASingleVariableSolutionReturnAValidSolution
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldMutateASingleVariableSolutionReturnAValidSolution()
   :outertype: PolynomialMutationTest

shouldMutateASingleVariableSolutionReturnAnotherValidSolution
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldMutateASingleVariableSolutionReturnAnotherValidSolution()
   :outertype: PolynomialMutationTest

shouldMutateASingleVariableSolutionReturnTheSameSolutionIfItIsNotMutated
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldMutateASingleVariableSolutionReturnTheSameSolutionIfItIsNotMutated()
   :outertype: PolynomialMutationTest

shouldMutateASingleVariableSolutionReturnTheSameSolutionIfProbabilityIsZero
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldMutateASingleVariableSolutionReturnTheSameSolutionIfProbabilityIsZero()
   :outertype: PolynomialMutationTest

shouldMutateASingleVariableSolutionWithSameLowerAndUpperBoundsReturnTheBoundValue
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldMutateASingleVariableSolutionWithSameLowerAndUpperBoundsReturnTheBoundValue()
   :outertype: PolynomialMutationTest

