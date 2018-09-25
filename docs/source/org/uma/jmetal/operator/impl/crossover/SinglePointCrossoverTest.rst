.. java:import:: org.junit Test

.. java:import:: org.mockito Mockito

.. java:import:: org.springframework.test.util ReflectionTestUtils

.. java:import:: org.uma.jmetal.problem BinaryProblem

.. java:import:: org.uma.jmetal.problem.impl AbstractBinaryProblem

.. java:import:: org.uma.jmetal.solution BinarySolution

.. java:import:: org.uma.jmetal.solution.impl DefaultBinarySolution

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: org.uma.jmetal.util.pseudorandom BoundedRandomGenerator

.. java:import:: org.uma.jmetal.util.pseudorandom JMetalRandom

.. java:import:: org.uma.jmetal.util.pseudorandom RandomGenerator

.. java:import:: org.uma.jmetal.util.pseudorandom.impl AuditableRandomGenerator

.. java:import:: java.util ArrayList

.. java:import:: java.util LinkedList

.. java:import:: java.util List

.. java:import:: java.util Random

SinglePointCrossoverTest
========================

.. java:package:: org.uma.jmetal.operator.impl.crossover
   :noindex:

.. java:type:: public class SinglePointCrossoverTest

Methods
-------
shouldConstructorAssignTheCorrectProbabilityValue
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldConstructorAssignTheCorrectProbabilityValue()
   :outertype: SinglePointCrossoverTest

shouldConstructorFailWhenPassedANegativeProbabilityValue
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldConstructorFailWhenPassedANegativeProbabilityValue()
   :outertype: SinglePointCrossoverTest

shouldCrossingTheBitInTheMiddleOfSecondVariableReturnTheCorrectCrossedSolutions
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldCrossingTheBitInTheMiddleOfSecondVariableReturnTheCorrectCrossedSolutions()
   :outertype: SinglePointCrossoverTest

shouldCrossingTheBitInTheMiddleOfTwoSingleVariableSolutionsReturnTheCorrectCrossedSolutions
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldCrossingTheBitInTheMiddleOfTwoSingleVariableSolutionsReturnTheCorrectCrossedSolutions()
   :outertype: SinglePointCrossoverTest

shouldCrossingTheFistBitOfSecondVariableReturnTheCorrectCrossedSolutions
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldCrossingTheFistBitOfSecondVariableReturnTheCorrectCrossedSolutions()
   :outertype: SinglePointCrossoverTest

shouldCrossingTheFistBitOfTwoSingleVariableSolutionsReturnTheCorrectCrossedSolutions
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldCrossingTheFistBitOfTwoSingleVariableSolutionsReturnTheCorrectCrossedSolutions()
   :outertype: SinglePointCrossoverTest

shouldCrossingTheLastBitOfTwoSingleVariableSolutionsReturnTheCorrectCrossedSolutions
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldCrossingTheLastBitOfTwoSingleVariableSolutionsReturnTheCorrectCrossedSolutions()
   :outertype: SinglePointCrossoverTest

shouldCrossingTwoVariableSolutionsReturnTheSameSolutionsIfNoBitsAreMutated
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldCrossingTwoVariableSolutionsReturnTheSameSolutionsIfNoBitsAreMutated()
   :outertype: SinglePointCrossoverTest

shouldExecuteFailIfTheListContainsMoreThanTwoSolutions
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldExecuteFailIfTheListContainsMoreThanTwoSolutions()
   :outertype: SinglePointCrossoverTest

shouldExecuteFailIfTheListContainsOnlyOneSolution
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldExecuteFailIfTheListContainsOnlyOneSolution()
   :outertype: SinglePointCrossoverTest

shouldExecuteWithNullParameterThrowAnException
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldExecuteWithNullParameterThrowAnException()
   :outertype: SinglePointCrossoverTest

shouldGetMutationProbabilityReturnTheRightValue
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldGetMutationProbabilityReturnTheRightValue()
   :outertype: SinglePointCrossoverTest

shouldJMetalRandomGeneratorNotBeUsedWhenCustomRandomGeneratorProvided
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldJMetalRandomGeneratorNotBeUsedWhenCustomRandomGeneratorProvided()
   :outertype: SinglePointCrossoverTest

