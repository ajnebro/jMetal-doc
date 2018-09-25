.. java:import:: org.uma.jmetal.problem DoubleProblem

.. java:import:: org.uma.jmetal.problem.impl AbstractDoubleProblem

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.solution.impl ArrayDoubleSolution

.. java:import:: org.uma.jmetal.util.archive Archive

.. java:import:: org.uma.jmetal.util.comparator DominanceComparator

.. java:import:: org.uma.jmetal.util.comparator EqualSolutionsComparator

.. java:import:: org.uma.jmetal.util.pseudorandom JMetalRandom

.. java:import:: java.util ArrayList

.. java:import:: java.util Comparator

.. java:import:: java.util Iterator

.. java:import:: java.util List

NonDominatedSolutionListArchive
===============================

.. java:package:: org.uma.jmetal.util.archive.impl
   :noindex:

.. java:type:: @SuppressWarnings public class NonDominatedSolutionListArchive<S extends Solution<?>> implements Archive<S>

   This class implements an archive containing non-dominated solutions

   :author: Antonio J. Nebro , Juan J. Durillo

Constructors
------------
NonDominatedSolutionListArchive
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public NonDominatedSolutionListArchive()
   :outertype: NonDominatedSolutionListArchive

   Constructor

NonDominatedSolutionListArchive
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public NonDominatedSolutionListArchive(DominanceComparator<S> comparator)
   :outertype: NonDominatedSolutionListArchive

   Constructor

Methods
-------
add
^^^

.. java:method:: @Override public boolean add(S solution)
   :outertype: NonDominatedSolutionListArchive

   Inserts a solution in the list

   :param solution: The solution to be inserted.
   :return: true if the operation success, and false if the solution is dominated or if an identical individual exists. The decision variables can be null if the solution is read from a file; in that case, the domination tests are omitted

get
^^^

.. java:method:: @Override public S get(int index)
   :outertype: NonDominatedSolutionListArchive

getSolutionList
^^^^^^^^^^^^^^^

.. java:method:: @Override public List<S> getSolutionList()
   :outertype: NonDominatedSolutionListArchive

join
^^^^

.. java:method:: public Archive<S> join(Archive<S> archive)
   :outertype: NonDominatedSolutionListArchive

main
^^^^

.. java:method:: public static void main(String[] args)
   :outertype: NonDominatedSolutionListArchive

size
^^^^

.. java:method:: @Override public int size()
   :outertype: NonDominatedSolutionListArchive

