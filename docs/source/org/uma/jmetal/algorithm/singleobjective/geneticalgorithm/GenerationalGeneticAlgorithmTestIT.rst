.. java:import:: org.junit Test

.. java:import:: org.uma.jmetal.algorithm Algorithm

.. java:import:: org.uma.jmetal.operator CrossoverOperator

.. java:import:: org.uma.jmetal.operator MutationOperator

.. java:import:: org.uma.jmetal.operator SelectionOperator

.. java:import:: org.uma.jmetal.operator.impl.crossover SinglePointCrossover

.. java:import:: org.uma.jmetal.operator.impl.mutation BitFlipMutation

.. java:import:: org.uma.jmetal.operator.impl.selection BinaryTournamentSelection

.. java:import:: org.uma.jmetal.problem BinaryProblem

.. java:import:: org.uma.jmetal.problem.singleobjective OneMax

.. java:import:: org.uma.jmetal.solution BinarySolution

.. java:import:: org.uma.jmetal.util AlgorithmRunner

.. java:import:: java.util List

GenerationalGeneticAlgorithmTestIT
==================================

.. java:package:: org.uma.jmetal.algorithm.singleobjective.geneticalgorithm
   :noindex:

.. java:type:: public class GenerationalGeneticAlgorithmTestIT

   Created by ajnebro on 27/10/15.

Methods
-------
shouldTheAlgorithmReturnTheCorrectSolutionWhenSolvingProblemOneMax
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldTheAlgorithmReturnTheCorrectSolutionWhenSolvingProblemOneMax()
   :outertype: GenerationalGeneticAlgorithmTestIT

