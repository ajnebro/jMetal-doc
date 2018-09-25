.. java:import:: org.junit Test

.. java:import:: org.mockito Mockito

.. java:import:: org.springframework.test.util ReflectionTestUtils

.. java:import:: org.uma.jmetal.problem BinaryProblem

.. java:import:: org.uma.jmetal.problem.impl AbstractBinaryProblem

.. java:import:: org.uma.jmetal.solution BinarySolution

.. java:import:: org.uma.jmetal.solution.impl DefaultBinarySolution

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: org.uma.jmetal.util.pseudorandom JMetalRandom

.. java:import:: org.uma.jmetal.util.pseudorandom RandomGenerator

.. java:import:: org.uma.jmetal.util.pseudorandom.impl AuditableRandomGenerator

.. java:import:: java.util Random

BitFlipMutationTest
===================

.. java:package:: org.uma.jmetal.operator.impl.mutation
   :noindex:

.. java:type:: public class BitFlipMutationTest

Methods
-------
shouldConstructorAssignTheCorrectProbabilityValue
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldConstructorAssignTheCorrectProbabilityValue()
   :outertype: BitFlipMutationTest

shouldConstructorFailWhenPassedANegativeProbabilityValue
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldConstructorFailWhenPassedANegativeProbabilityValue()
   :outertype: BitFlipMutationTest

shouldExecuteWithNullParameterThrowAnException
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldExecuteWithNullParameterThrowAnException()
   :outertype: BitFlipMutationTest

shouldGetMutationProbabilityReturnTheRightValue
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldGetMutationProbabilityReturnTheRightValue()
   :outertype: BitFlipMutationTest

shouldJMetalRandomGeneratorNotBeUsedWhenCustomRandomGeneratorProvided
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldJMetalRandomGeneratorNotBeUsedWhenCustomRandomGeneratorProvided()
   :outertype: BitFlipMutationTest

shouldMutateASingleVariableSolutionReturnTheSameSolutionIfNoBitsAreMutated
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldMutateASingleVariableSolutionReturnTheSameSolutionIfNoBitsAreMutated()
   :outertype: BitFlipMutationTest

shouldMutateASingleVariableSolutionWhenASingleBitIsMutated
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldMutateASingleVariableSolutionWhenASingleBitIsMutated()
   :outertype: BitFlipMutationTest

shouldMutateATwoVariableSolutionReturnTheSameSolutionIfNoBitsAreMutated
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldMutateATwoVariableSolutionReturnTheSameSolutionIfNoBitsAreMutated()
   :outertype: BitFlipMutationTest

shouldMutateATwoVariableSolutionWhenTwoBitsAreMutated
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldMutateATwoVariableSolutionWhenTwoBitsAreMutated()
   :outertype: BitFlipMutationTest

