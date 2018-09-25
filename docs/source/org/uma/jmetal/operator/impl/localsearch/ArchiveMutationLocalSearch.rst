.. java:import:: org.uma.jmetal.operator LocalSearchOperator

.. java:import:: org.uma.jmetal.operator MutationOperator

.. java:import:: org.uma.jmetal.problem ConstrainedProblem

.. java:import:: org.uma.jmetal.problem Problem

.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util.archive Archive

.. java:import:: org.uma.jmetal.util.comparator DominanceComparator

.. java:import:: org.uma.jmetal.util.comparator.impl OverallConstraintViolationComparator

.. java:import:: java.util Comparator

ArchiveMutationLocalSearch
==========================

.. java:package:: org.uma.jmetal.operator.impl.localsearch
   :noindex:

.. java:type:: @SuppressWarnings public class ArchiveMutationLocalSearch<S extends Solution<?>> implements LocalSearchOperator<S>

   This class implements a local search operator based in the use of a mutation operator. An archive is used to store the non-dominated solutions found during the search.

   :author: Antonio J. Nebro

Constructors
------------
ArchiveMutationLocalSearch
^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public ArchiveMutationLocalSearch(int improvementRounds, MutationOperator<S> mutationOperator, Archive<S> archive, Problem<S> problem)
   :outertype: ArchiveMutationLocalSearch

   Constructor. Creates a new local search object.

   :param improvementRounds: number of iterations
   :param mutationOperator: mutation operator
   :param archive: archive to store non-dominated solution
   :param problem: problem to resolve

Methods
-------
execute
^^^^^^^

.. java:method:: @SuppressWarnings public S execute(S solution)
   :outertype: ArchiveMutationLocalSearch

   Executes the local search.

   :param solution: The solution to improve
   :return: The improved solution

getEvaluations
^^^^^^^^^^^^^^

.. java:method:: public int getEvaluations()
   :outertype: ArchiveMutationLocalSearch

   Returns the number of evaluations

getNumberOfImprovements
^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public int getNumberOfImprovements()
   :outertype: ArchiveMutationLocalSearch

getNumberOfNonComparableSolutions
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public int getNumberOfNonComparableSolutions()
   :outertype: ArchiveMutationLocalSearch

