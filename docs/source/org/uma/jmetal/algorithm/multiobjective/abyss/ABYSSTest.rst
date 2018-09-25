.. java:import:: org.junit Before

.. java:import:: org.junit Test

.. java:import:: org.springframework.test.util ReflectionTestUtils

.. java:import:: org.uma.jmetal.algorithm.multiobjective.abyss.util MarkAttribute

.. java:import:: org.uma.jmetal.operator LocalSearchOperator

.. java:import:: org.uma.jmetal.operator MutationOperator

.. java:import:: org.uma.jmetal.operator.impl.crossover SBXCrossover

.. java:import:: org.uma.jmetal.operator.impl.localsearch ArchiveMutationLocalSearch

.. java:import:: org.uma.jmetal.operator.impl.mutation PolynomialMutation

.. java:import:: org.uma.jmetal.problem DoubleProblem

.. java:import:: org.uma.jmetal.problem.impl AbstractDoubleProblem

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.solution.impl DefaultDoubleSolution

.. java:import:: org.uma.jmetal.util.archive Archive

.. java:import:: org.uma.jmetal.util.archive.impl CrowdingDistanceArchive

.. java:import:: org.uma.jmetal.util.pseudorandom JMetalRandom

.. java:import:: java.util ArrayList

.. java:import:: java.util List

ABYSSTest
=========

.. java:package:: org.uma.jmetal.algorithm.multiobjective.abyss
   :noindex:

.. java:type:: public class ABYSSTest

   Created by ajnebro on 11/6/15.

Fields
------
archive
^^^^^^^

.. java:field::  Archive<DoubleSolution> archive
   :outertype: ABYSSTest

localSearch
^^^^^^^^^^^

.. java:field::  LocalSearchOperator<DoubleSolution> localSearch
   :outertype: ABYSSTest

mutation
^^^^^^^^

.. java:field::  MutationOperator<DoubleSolution> mutation
   :outertype: ABYSSTest

problem
^^^^^^^

.. java:field::  DoubleProblem problem
   :outertype: ABYSSTest

Methods
-------
setup
^^^^^

.. java:method:: @Before public void setup()
   :outertype: ABYSSTest

shouldInitializationPhaseLeadToAPopulationFilledWithEvaluatedSolutions
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldInitializationPhaseLeadToAPopulationFilledWithEvaluatedSolutions()
   :outertype: ABYSSTest

shouldIsStoppingConditionReachedReturnFalseIfTheConditionDoesNotFulfill
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldIsStoppingConditionReachedReturnFalseIfTheConditionDoesNotFulfill()
   :outertype: ABYSSTest

shouldIsStoppingConditionReachedReturnTrueIfTheConditionFulfills
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldIsStoppingConditionReachedReturnTrueIfTheConditionFulfills()
   :outertype: ABYSSTest

shouldReferenceSetUpdateCreateAReducedSizeReferenceSet2IfThePopulationIsNotBigEnough
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldReferenceSetUpdateCreateAReducedSizeReferenceSet2IfThePopulationIsNotBigEnough()
   :outertype: ABYSSTest

shouldReferenceSetUpdateCreateTheTwoRefSetsAfterBeingInvokedTheFirstTime
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldReferenceSetUpdateCreateTheTwoRefSetsAfterBeingInvokedTheFirstTime()
   :outertype: ABYSSTest

shouldRestartCreateANewPopulationWithTheRefSet1Solutions
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldRestartCreateANewPopulationWithTheRefSet1Solutions()
   :outertype: ABYSSTest

shouldSolutionCombinationProduceTheRightNumberOfSolutions
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldSolutionCombinationProduceTheRightNumberOfSolutions()
   :outertype: ABYSSTest

shouldSubsetGenerationProduceAnEmptyListIfAllTheSolutionsAreMarked
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldSubsetGenerationProduceAnEmptyListIfAllTheSolutionsAreMarked()
   :outertype: ABYSSTest

