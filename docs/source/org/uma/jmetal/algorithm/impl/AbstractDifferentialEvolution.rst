.. java:import:: org.uma.jmetal.operator.impl.crossover DifferentialEvolutionCrossover

.. java:import:: org.uma.jmetal.operator.impl.selection DifferentialEvolutionSelection

.. java:import:: org.uma.jmetal.solution DoubleSolution

AbstractDifferentialEvolution
=============================

.. java:package:: org.uma.jmetal.algorithm.impl
   :noindex:

.. java:type:: @SuppressWarnings public abstract class AbstractDifferentialEvolution<Result> extends AbstractEvolutionaryAlgorithm<DoubleSolution, Result>

   Abstract class representing differential evolution (DE) algorithms

   :author: Antonio J. Nebro

Fields
------
crossoverOperator
^^^^^^^^^^^^^^^^^

.. java:field:: protected DifferentialEvolutionCrossover crossoverOperator
   :outertype: AbstractDifferentialEvolution

selectionOperator
^^^^^^^^^^^^^^^^^

.. java:field:: protected DifferentialEvolutionSelection selectionOperator
   :outertype: AbstractDifferentialEvolution

