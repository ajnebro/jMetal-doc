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

SBXCrossoverTest
================

.. java:package:: org.uma.jmetal.operator.impl.crossover
   :noindex:

.. java:type:: public class SBXCrossoverTest

   Note: this class does check that the SBX crossover operator does not return invalid values, but not that it works properly (@see SBXCrossoverWorkingTest)

   :author: Antonio J. Nebro

Methods
-------
shouldConstructorAssignTheCorrectDistributionIndex
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldConstructorAssignTheCorrectDistributionIndex()
   :outertype: SBXCrossoverTest

shouldConstructorAssignTheCorrectProbabilityValue
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldConstructorAssignTheCorrectProbabilityValue()
   :outertype: SBXCrossoverTest

shouldConstructorFailWhenPassedANegativeDistributionIndex
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldConstructorFailWhenPassedANegativeDistributionIndex()
   :outertype: SBXCrossoverTest

shouldConstructorFailWhenPassedANegativeProbabilityValue
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldConstructorFailWhenPassedANegativeProbabilityValue()
   :outertype: SBXCrossoverTest

shouldCrossingTheSecondVariableReturnTheOtherVariablesUnchangedInTheOffspringSolutions
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldCrossingTheSecondVariableReturnTheOtherVariablesUnchangedInTheOffspringSolutions()
   :outertype: SBXCrossoverTest

shouldCrossingTwoDoubleVariableSolutionsReturnValidSolutions
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldCrossingTwoDoubleVariableSolutionsReturnValidSolutions()
   :outertype: SBXCrossoverTest

shouldCrossingTwoSingleVariableSolutionsReturnTheSameSolutionsIfNotCrossoverIsApplied
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldCrossingTwoSingleVariableSolutionsReturnTheSameSolutionsIfNotCrossoverIsApplied()
   :outertype: SBXCrossoverTest

shouldCrossingTwoSingleVariableSolutionsReturnTheSameSolutionsIfProbabilityIsZero
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldCrossingTwoSingleVariableSolutionsReturnTheSameSolutionsIfProbabilityIsZero()
   :outertype: SBXCrossoverTest

shouldCrossingTwoSingleVariableSolutionsReturnValidSolutions
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldCrossingTwoSingleVariableSolutionsReturnValidSolutions()
   :outertype: SBXCrossoverTest

shouldCrossingTwoSingleVariableSolutionsWithSimilarValueReturnTheSameVariables
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldCrossingTwoSingleVariableSolutionsWithSimilarValueReturnTheSameVariables()
   :outertype: SBXCrossoverTest

shouldExecuteWithInvalidSolutionListSizeThrowAnException
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldExecuteWithInvalidSolutionListSizeThrowAnException()
   :outertype: SBXCrossoverTest

shouldExecuteWithNullParameterThrowAnException
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldExecuteWithNullParameterThrowAnException()
   :outertype: SBXCrossoverTest

shouldGetDistributionIndexReturnTheRightValue
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldGetDistributionIndexReturnTheRightValue()
   :outertype: SBXCrossoverTest

shouldGetProbabilityReturnTheRightValue
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldGetProbabilityReturnTheRightValue()
   :outertype: SBXCrossoverTest

shouldJMetalRandomGeneratorNotBeUsedWhenCustomRandomGeneratorProvided
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldJMetalRandomGeneratorNotBeUsedWhenCustomRandomGeneratorProvided()
   :outertype: SBXCrossoverTest

