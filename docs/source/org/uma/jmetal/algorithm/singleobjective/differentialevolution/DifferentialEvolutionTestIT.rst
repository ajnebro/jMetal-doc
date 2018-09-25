.. java:import:: junit.framework TestCase

.. java:import:: org.junit Assert

.. java:import:: org.junit Before

.. java:import:: org.junit Test

.. java:import:: org.junit.runner RunWith

.. java:import:: org.mockito Mock

.. java:import:: org.mockito Mockito

.. java:import:: org.mockito.runners MockitoJUnitRunner

.. java:import:: org.springframework.test.util ReflectionTestUtils

.. java:import:: org.uma.jmetal.operator.impl.crossover DifferentialEvolutionCrossover

.. java:import:: org.uma.jmetal.operator.impl.selection DifferentialEvolutionSelection

.. java:import:: org.uma.jmetal.problem DoubleProblem

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.util.evaluator.impl SequentialSolutionListEvaluator

.. java:import:: java.util Arrays

.. java:import:: java.util List

DifferentialEvolutionTestIT
===========================

.. java:package:: org.uma.jmetal.algorithm.singleobjective.differentialevolution
   :noindex:

.. java:type:: @RunWith public class DifferentialEvolutionTestIT

   Created by Antonio J. Nebro on 25/11/14.

Methods
-------
shouldCreateInitialPopulationWhenPopulationSizeIsBiggerThanZero
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldCreateInitialPopulationWhenPopulationSizeIsBiggerThanZero()
   :outertype: DifferentialEvolutionTestIT

shouldCreateInitialPopulationWhenPopulationSizeIsZero
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldCreateInitialPopulationWhenPopulationSizeIsZero()
   :outertype: DifferentialEvolutionTestIT

shouldEvaluatePopulation
^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldEvaluatePopulation()
   :outertype: DifferentialEvolutionTestIT

shouldGetEvaluations
^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldGetEvaluations()
   :outertype: DifferentialEvolutionTestIT

shouldGetResultReturnsThenReturnTheBestIndividual
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldGetResultReturnsThenReturnTheBestIndividual()
   :outertype: DifferentialEvolutionTestIT

shouldInitProgress
^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldInitProgress()
   :outertype: DifferentialEvolutionTestIT

shouldIsStoppingConditionReachedWhenEvaluationsBiggerThenMaxEvaluations
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldIsStoppingConditionReachedWhenEvaluationsBiggerThenMaxEvaluations()
   :outertype: DifferentialEvolutionTestIT

shouldIsStoppingConditionReachedWhenEvaluationsEqualToMaxEvaluations
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldIsStoppingConditionReachedWhenEvaluationsEqualToMaxEvaluations()
   :outertype: DifferentialEvolutionTestIT

shouldIsStoppingConditionReachedWhenEvaluationsLesserThanMaxEvaluations
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldIsStoppingConditionReachedWhenEvaluationsLesserThanMaxEvaluations()
   :outertype: DifferentialEvolutionTestIT

shouldReplacemen2t
^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldReplacemen2t()
   :outertype: DifferentialEvolutionTestIT

shouldReproduction
^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldReproduction()
   :outertype: DifferentialEvolutionTestIT

shouldSelection
^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldSelection()
   :outertype: DifferentialEvolutionTestIT

shouldSetEvaluations
^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldSetEvaluations()
   :outertype: DifferentialEvolutionTestIT

shouldUpdateProgressWhenAnyIteration
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldUpdateProgressWhenAnyIteration()
   :outertype: DifferentialEvolutionTestIT

shouldUpdateProgressWhenFirstIteration
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldUpdateProgressWhenFirstIteration()
   :outertype: DifferentialEvolutionTestIT

startup
^^^^^^^

.. java:method:: @Before public void startup()
   :outertype: DifferentialEvolutionTestIT

