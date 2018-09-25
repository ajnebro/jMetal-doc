.. java:import:: org.uma.jmetal.operator SelectionOperator

.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: org.uma.jmetal.util SolutionListUtils

.. java:import:: org.uma.jmetal.util.comparator DominanceComparator

.. java:import:: java.util Comparator

.. java:import:: java.util List

NaryTournamentSelection
=======================

.. java:package:: org.uma.jmetal.operator.impl.selection
   :noindex:

.. java:type:: @SuppressWarnings public class NaryTournamentSelection<S extends Solution<?>> implements SelectionOperator<List<S>, S>

   Applies a N-ary tournament selection to return the best solution between N that have been chosen at random from a solution list.

   :author: Antonio J. Nebro

Constructors
------------
NaryTournamentSelection
^^^^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public NaryTournamentSelection()
   :outertype: NaryTournamentSelection

   Constructor

NaryTournamentSelection
^^^^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public NaryTournamentSelection(int numberOfSolutionsToBeReturned, Comparator<S> comparator)
   :outertype: NaryTournamentSelection

   Constructor

Methods
-------
execute
^^^^^^^

.. java:method:: @Override public S execute(List<S> solutionList)
   :outertype: NaryTournamentSelection

