.. java:import:: org.uma.jmetal.operator CrossoverOperator

.. java:import:: org.uma.jmetal.operator MutationOperator

.. java:import:: org.uma.jmetal.operator SelectionOperator

.. java:import:: org.uma.jmetal.problem Problem

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: java.util ArrayList

.. java:import:: java.util List

AbstractGeneticAlgorithm
========================

.. java:package:: org.uma.jmetal.algorithm.impl
   :noindex:

.. java:type:: @SuppressWarnings public abstract class AbstractGeneticAlgorithm<S, Result> extends AbstractEvolutionaryAlgorithm<S, Result>

   Abstract class representing a genetic algorithm

   :author: Antonio J. Nebro

Fields
------
crossoverOperator
^^^^^^^^^^^^^^^^^

.. java:field:: protected CrossoverOperator<S> crossoverOperator
   :outertype: AbstractGeneticAlgorithm

maxPopulationSize
^^^^^^^^^^^^^^^^^

.. java:field:: protected int maxPopulationSize
   :outertype: AbstractGeneticAlgorithm

mutationOperator
^^^^^^^^^^^^^^^^

.. java:field:: protected MutationOperator<S> mutationOperator
   :outertype: AbstractGeneticAlgorithm

selectionOperator
^^^^^^^^^^^^^^^^^

.. java:field:: protected SelectionOperator<List<S>, S> selectionOperator
   :outertype: AbstractGeneticAlgorithm

Constructors
------------
AbstractGeneticAlgorithm
^^^^^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public AbstractGeneticAlgorithm(Problem<S> problem)
   :outertype: AbstractGeneticAlgorithm

   Constructor

   :param problem: The problem to solve

Methods
-------
checkNumberOfParents
^^^^^^^^^^^^^^^^^^^^

.. java:method:: protected void checkNumberOfParents(List<S> population, int numberOfParentsForCrossover)
   :outertype: AbstractGeneticAlgorithm

   A crossover operator is applied to a number of parents, and it assumed that the population contains a valid number of solutions. This method checks that.

   :param population:
   :param numberOfParentsForCrossover:

createInitialPopulation
^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: protected List<S> createInitialPopulation()
   :outertype: AbstractGeneticAlgorithm

   This method implements a default scheme create the initial population of genetic algorithm

getCrossoverOperator
^^^^^^^^^^^^^^^^^^^^

.. java:method:: public CrossoverOperator<S> getCrossoverOperator()
   :outertype: AbstractGeneticAlgorithm

getMaxPopulationSize
^^^^^^^^^^^^^^^^^^^^

.. java:method:: public int getMaxPopulationSize()
   :outertype: AbstractGeneticAlgorithm

getMutationOperator
^^^^^^^^^^^^^^^^^^^

.. java:method:: public MutationOperator<S> getMutationOperator()
   :outertype: AbstractGeneticAlgorithm

getSelectionOperator
^^^^^^^^^^^^^^^^^^^^

.. java:method:: public SelectionOperator<List<S>, S> getSelectionOperator()
   :outertype: AbstractGeneticAlgorithm

reproduction
^^^^^^^^^^^^

.. java:method:: @Override protected List<S> reproduction(List<S> population)
   :outertype: AbstractGeneticAlgorithm

   This methods iteratively applies a \ :java:ref:`CrossoverOperator`\  a \ :java:ref:`MutationOperator`\  to the population to create the offspring population. The population size must be divisible by the number of parents required by the \ :java:ref:`CrossoverOperator`\ ; this way, the needed parents are taken sequentially from the population. No limits are imposed to the number of solutions returned by the \ :java:ref:`CrossoverOperator`\ .

   :param population:
   :return: The new created offspring population

selection
^^^^^^^^^

.. java:method:: @Override protected List<S> selection(List<S> population)
   :outertype: AbstractGeneticAlgorithm

   This method iteratively applies a \ :java:ref:`SelectionOperator`\  to the population to fill the mating pool population.

   :param population:
   :return: The mating pool population

setMaxPopulationSize
^^^^^^^^^^^^^^^^^^^^

.. java:method:: public void setMaxPopulationSize(int maxPopulationSize)
   :outertype: AbstractGeneticAlgorithm

