.. java:import:: org.uma.jmetal.operator LocalSearchOperator

.. java:import:: org.uma.jmetal.operator MutationOperator

.. java:import:: org.uma.jmetal.problem ConstrainedProblem

.. java:import:: org.uma.jmetal.problem Problem

.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util.comparator.impl OverallConstraintViolationComparator

.. java:import:: org.uma.jmetal.util.pseudorandom JMetalRandom

.. java:import:: org.uma.jmetal.util.pseudorandom RandomGenerator

.. java:import:: java.util Comparator

BasicLocalSearch
================

.. java:package:: org.uma.jmetal.operator.impl.localsearch
   :noindex:

.. java:type:: @SuppressWarnings public class BasicLocalSearch<S extends Solution<?>> implements LocalSearchOperator<S>

   This class implements a basic local search operator based in the use of a mutation operator.

   :author: Antonio J. Nebro

Constructors
------------
BasicLocalSearch
^^^^^^^^^^^^^^^^

.. java:constructor:: public BasicLocalSearch(int improvementRounds, MutationOperator<S> mutationOperator, Comparator<S> comparator, Problem<S> problem)
   :outertype: BasicLocalSearch

   Constructor. Creates a new local search object.

   :param improvementRounds: number of iterations
   :param mutationOperator: mutation operator
   :param comparator: comparator to determine which solution is the best
   :param problem: problem to resolve

BasicLocalSearch
^^^^^^^^^^^^^^^^

.. java:constructor:: public BasicLocalSearch(int improvementRounds, MutationOperator<S> mutationOperator, Comparator<S> comparator, Problem<S> problem, RandomGenerator<Double> randomGenerator)
   :outertype: BasicLocalSearch

   Constructor. Creates a new local search object.

   :param improvementRounds: number of iterations
   :param mutationOperator: mutation operator
   :param comparator: comparator to determine which solution is the best
   :param problem: problem to resolve
   :param randomGenerator: the \ :java:ref:`RandomGenerator`\  to use when we must choose between equivalent solutions

Methods
-------
execute
^^^^^^^

.. java:method:: @SuppressWarnings public S execute(S solution)
   :outertype: BasicLocalSearch

   Executes the local search.

   :param solution: The solution to improve
   :return: An improved solution

getEvaluations
^^^^^^^^^^^^^^

.. java:method:: public int getEvaluations()
   :outertype: BasicLocalSearch

   Returns the number of evaluations

getNumberOfImprovements
^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public int getNumberOfImprovements()
   :outertype: BasicLocalSearch

getNumberOfNonComparableSolutions
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public int getNumberOfNonComparableSolutions()
   :outertype: BasicLocalSearch

