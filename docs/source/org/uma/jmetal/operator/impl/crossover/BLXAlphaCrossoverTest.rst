.. java:import:: org.hamcrest Matchers

.. java:import:: org.junit Test

.. java:import:: org.mockito Mockito

.. java:import:: org.springframework.test.util ReflectionTestUtils

.. java:import:: org.uma.jmetal.problem DoubleProblem

.. java:import:: org.uma.jmetal.problem.impl AbstractDoubleProblem

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.solution.util RepairDoubleSolutionAtBounds

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: org.uma.jmetal.util.pseudorandom JMetalRandom

.. java:import:: org.uma.jmetal.util.pseudorandom RandomGenerator

.. java:import:: org.uma.jmetal.util.pseudorandom.impl AuditableRandomGenerator

BLXAlphaCrossoverTest
=====================

.. java:package:: org.uma.jmetal.operator.impl.crossover
   :noindex:

.. java:type:: public class BLXAlphaCrossoverTest

   Note: this class does check that the BLX-aplha crossover operator does not return invalid values, but not that it works properly (@see BLXAlphaCrossoverWorkingTest)

   :author: Antonio J. Nebro

Methods
-------
shouldConstructorAssignTheCorrectDistributionIndex
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldConstructorAssignTheCorrectDistributionIndex()
   :outertype: BLXAlphaCrossoverTest

shouldConstructorAssignTheCorrectProbabilityValue
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldConstructorAssignTheCorrectProbabilityValue()
   :outertype: BLXAlphaCrossoverTest

shouldConstructorFailWhenPassedANegativeAlphaValue
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldConstructorFailWhenPassedANegativeAlphaValue()
   :outertype: BLXAlphaCrossoverTest

shouldConstructorFailWhenPassedANegativeProbabilityValue
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldConstructorFailWhenPassedANegativeProbabilityValue()
   :outertype: BLXAlphaCrossoverTest

shouldCrossingTwoDoubleVariableSolutionsReturnValidSolutions
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldCrossingTwoDoubleVariableSolutionsReturnValidSolutions()
   :outertype: BLXAlphaCrossoverTest

shouldCrossingTwoSingleVariableSolutionsReturnTheSameSolutionsIfNotCrossoverIsApplied
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldCrossingTwoSingleVariableSolutionsReturnTheSameSolutionsIfNotCrossoverIsApplied()
   :outertype: BLXAlphaCrossoverTest

shouldCrossingTwoSingleVariableSolutionsReturnTheSameSolutionsIfProbabilityIsZero
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldCrossingTwoSingleVariableSolutionsReturnTheSameSolutionsIfProbabilityIsZero()
   :outertype: BLXAlphaCrossoverTest

shouldCrossingTwoSingleVariableSolutionsReturnValidSolutions
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldCrossingTwoSingleVariableSolutionsReturnValidSolutions()
   :outertype: BLXAlphaCrossoverTest

shouldCrossingTwoSingleVariableSolutionsWithSimilarValueReturnTheSameVariables
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldCrossingTwoSingleVariableSolutionsWithSimilarValueReturnTheSameVariables()
   :outertype: BLXAlphaCrossoverTest

shouldExecuteWithInvalidSolutionListSizeThrowAnException
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldExecuteWithInvalidSolutionListSizeThrowAnException()
   :outertype: BLXAlphaCrossoverTest

shouldExecuteWithNullParameterThrowAnException
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldExecuteWithNullParameterThrowAnException()
   :outertype: BLXAlphaCrossoverTest

shouldGetAlphaReturnTheRightValue
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldGetAlphaReturnTheRightValue()
   :outertype: BLXAlphaCrossoverTest

shouldGetProbabilityReturnTheRightValue
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldGetProbabilityReturnTheRightValue()
   :outertype: BLXAlphaCrossoverTest

shouldJMetalRandomGeneratorNotBeUsedWhenCustomRandomGeneratorProvided
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldJMetalRandomGeneratorNotBeUsedWhenCustomRandomGeneratorProvided()
   :outertype: BLXAlphaCrossoverTest

