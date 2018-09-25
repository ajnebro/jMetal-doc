.. java:import:: org.junit Ignore

.. java:import:: org.junit Test

.. java:import:: org.uma.jmetal.algorithm Algorithm

.. java:import:: org.uma.jmetal.operator CrossoverOperator

.. java:import:: org.uma.jmetal.operator MutationOperator

.. java:import:: org.uma.jmetal.operator SelectionOperator

.. java:import:: org.uma.jmetal.operator.impl.crossover SBXCrossover

.. java:import:: org.uma.jmetal.operator.impl.mutation PolynomialMutation

.. java:import:: org.uma.jmetal.operator.impl.selection BinaryTournamentSelection

.. java:import:: org.uma.jmetal.problem DoubleProblem

.. java:import:: org.uma.jmetal.problem.multiobjective.zdt ZDT1

.. java:import:: org.uma.jmetal.qualityindicator QualityIndicator

.. java:import:: org.uma.jmetal.qualityindicator.impl.hypervolume PISAHypervolume

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.util.comparator RankingAndCrowdingDistanceComparator

.. java:import:: org.uma.jmetal.util.evaluator.impl SequentialSolutionListEvaluator

.. java:import:: java.util ArrayList

.. java:import:: java.util List

WASFGAIT
========

.. java:package:: org.uma.jmetal.algorithm.multiobjective.wasfga
   :noindex:

.. java:type:: public class WASFGAIT

Methods
-------
shouldTheAlgorithmReturnANumberOfSolutionsWhenSolvingASimpleProblem
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldTheAlgorithmReturnANumberOfSolutionsWhenSolvingASimpleProblem() throws Exception
   :outertype: WASFGAIT

shouldTheAlgorithmReturnAnExceptionIfIndicatingANonExistingWeightVectorFile
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test @Ignore public void shouldTheAlgorithmReturnAnExceptionIfIndicatingANonExistingWeightVectorFile()
   :outertype: WASFGAIT

shouldTheHypervolumeHaveAMininumValue
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldTheHypervolumeHaveAMininumValue() throws Exception
   :outertype: WASFGAIT

