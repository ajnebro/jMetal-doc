.. java:import:: org.junit Before

.. java:import:: org.junit Test

.. java:import:: org.uma.jmetal.algorithm Algorithm

.. java:import:: org.uma.jmetal.operator CrossoverOperator

.. java:import:: org.uma.jmetal.operator LocalSearchOperator

.. java:import:: org.uma.jmetal.operator MutationOperator

.. java:import:: org.uma.jmetal.operator.impl.crossover SBXCrossover

.. java:import:: org.uma.jmetal.operator.impl.localsearch ArchiveMutationLocalSearch

.. java:import:: org.uma.jmetal.operator.impl.mutation PolynomialMutation

.. java:import:: org.uma.jmetal.problem DoubleProblem

.. java:import:: org.uma.jmetal.problem.multiobjective.zdt ZDT4

.. java:import:: org.uma.jmetal.qualityindicator QualityIndicator

.. java:import:: org.uma.jmetal.qualityindicator.impl.hypervolume PISAHypervolume

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.util AlgorithmRunner

.. java:import:: org.uma.jmetal.util.archive Archive

.. java:import:: org.uma.jmetal.util.archive.impl CrowdingDistanceArchive

.. java:import:: java.util List

ABYSSIT
=======

.. java:package:: org.uma.jmetal.algorithm.multiobjective.abyss
   :noindex:

.. java:type:: public class ABYSSIT

   Created by ajnebro on 11/6/15.

Fields
------
algorithm
^^^^^^^^^

.. java:field::  Algorithm<List<DoubleSolution>> algorithm
   :outertype: ABYSSIT

archive
^^^^^^^

.. java:field::  Archive<DoubleSolution> archive
   :outertype: ABYSSIT

crossover
^^^^^^^^^

.. java:field::  CrossoverOperator<DoubleSolution> crossover
   :outertype: ABYSSIT

localSearchOperator
^^^^^^^^^^^^^^^^^^^

.. java:field::  LocalSearchOperator<DoubleSolution> localSearchOperator
   :outertype: ABYSSIT

mutation
^^^^^^^^

.. java:field::  MutationOperator<DoubleSolution> mutation
   :outertype: ABYSSIT

problem
^^^^^^^

.. java:field::  DoubleProblem problem
   :outertype: ABYSSIT

Methods
-------
setup
^^^^^

.. java:method:: @Before public void setup()
   :outertype: ABYSSIT

shouldTheAlgorithmReturnANumberOfSolutionsWhenSolvingASimpleProblem
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldTheAlgorithmReturnANumberOfSolutionsWhenSolvingASimpleProblem() throws Exception
   :outertype: ABYSSIT

shouldTheHypervolumeHaveAMininumValue
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldTheHypervolumeHaveAMininumValue() throws Exception
   :outertype: ABYSSIT

