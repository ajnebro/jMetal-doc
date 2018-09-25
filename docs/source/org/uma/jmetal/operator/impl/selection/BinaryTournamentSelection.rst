.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util.comparator DominanceComparator

.. java:import:: java.util Comparator

BinaryTournamentSelection
=========================

.. java:package:: org.uma.jmetal.operator.impl.selection
   :noindex:

.. java:type:: @SuppressWarnings public class BinaryTournamentSelection<S extends Solution<?>> extends TournamentSelection<S>

   Applies a binary tournament selection to return the best solution between two that have been chosen at random from a solution list. Modified by Juanjo in 13.03.2015. A binary tournament is now a TournamenteSelection with 2 tournaments

   :author: Antonio J. Nebro, Juan J. Durillo

Constructors
------------
BinaryTournamentSelection
^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public BinaryTournamentSelection()
   :outertype: BinaryTournamentSelection

   Constructor

BinaryTournamentSelection
^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public BinaryTournamentSelection(Comparator<S> comparator)
   :outertype: BinaryTournamentSelection

   Constructor

