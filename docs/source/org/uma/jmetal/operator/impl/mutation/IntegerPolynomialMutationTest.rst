.. java:import:: org.hamcrest Matchers

.. java:import:: org.junit Test

.. java:import:: org.mockito Mockito

.. java:import:: org.springframework.test.util ReflectionTestUtils

.. java:import:: org.uma.jmetal.problem IntegerProblem

.. java:import:: org.uma.jmetal.problem.impl AbstractIntegerProblem

.. java:import:: org.uma.jmetal.solution IntegerSolution

.. java:import:: org.uma.jmetal.solution.impl DefaultIntegerSolution

.. java:import:: org.uma.jmetal.solution.util RepairDoubleSolutionAtBounds

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: org.uma.jmetal.util.pseudorandom JMetalRandom

.. java:import:: org.uma.jmetal.util.pseudorandom RandomGenerator

.. java:import:: org.uma.jmetal.util.pseudorandom.impl AuditableRandomGenerator

.. java:import:: java.util ArrayList

.. java:import:: java.util Arrays

.. java:import:: java.util List

.. java:import:: java.util Random

IntegerPolynomialMutationTest
=============================

.. java:package:: org.uma.jmetal.operator.impl.mutation
   :noindex:

.. java:type:: public class IntegerPolynomialMutationTest

Methods
-------
shouldConstructorAssignTheCorrectDistributionIndex
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldConstructorAssignTheCorrectDistributionIndex()
   :outertype: IntegerPolynomialMutationTest

shouldConstructorAssignTheCorrectProbabilityValue
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldConstructorAssignTheCorrectProbabilityValue()
   :outertype: IntegerPolynomialMutationTest

shouldConstructorFailWhenPassedANegativeDistributionIndex
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldConstructorFailWhenPassedANegativeDistributionIndex()
   :outertype: IntegerPolynomialMutationTest

shouldConstructorFailWhenPassedANegativeProbabilityValue
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldConstructorFailWhenPassedANegativeProbabilityValue()
   :outertype: IntegerPolynomialMutationTest

shouldConstructorWithProblemAndDistributionIndexParametersAssignTheCorrectValues
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldConstructorWithProblemAndDistributionIndexParametersAssignTheCorrectValues()
   :outertype: IntegerPolynomialMutationTest

shouldConstructorWithoutParameterAssignTheDefaultValues
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldConstructorWithoutParameterAssignTheDefaultValues()
   :outertype: IntegerPolynomialMutationTest

shouldExecuteWithNullParameterThrowAnException
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldExecuteWithNullParameterThrowAnException()
   :outertype: IntegerPolynomialMutationTest

shouldGetDistributionIndexReturnTheRightValue
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldGetDistributionIndexReturnTheRightValue()
   :outertype: IntegerPolynomialMutationTest

shouldGetMutationProbabilityReturnTheRightValue
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldGetMutationProbabilityReturnTheRightValue()
   :outertype: IntegerPolynomialMutationTest

shouldJMetalRandomGeneratorNotBeUsedWhenCustomRandomGeneratorProvided
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldJMetalRandomGeneratorNotBeUsedWhenCustomRandomGeneratorProvided()
   :outertype: IntegerPolynomialMutationTest

shouldMutateASingleVariableSolutionReturnAValidSolution
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldMutateASingleVariableSolutionReturnAValidSolution()
   :outertype: IntegerPolynomialMutationTest

shouldMutateASingleVariableSolutionReturnAnotherValidSolution
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldMutateASingleVariableSolutionReturnAnotherValidSolution()
   :outertype: IntegerPolynomialMutationTest

shouldMutateASingleVariableSolutionReturnTheSameSolutionIfItIsNotMutated
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldMutateASingleVariableSolutionReturnTheSameSolutionIfItIsNotMutated()
   :outertype: IntegerPolynomialMutationTest

shouldMutateASingleVariableSolutionReturnTheSameSolutionIfProbabilityIsZero
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldMutateASingleVariableSolutionReturnTheSameSolutionIfProbabilityIsZero()
   :outertype: IntegerPolynomialMutationTest

shouldMutateASingleVariableSolutionWithSameLowerAndUpperBoundsReturnTheBoundValue
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldMutateASingleVariableSolutionWithSameLowerAndUpperBoundsReturnTheBoundValue()
   :outertype: IntegerPolynomialMutationTest

