.. java:import:: org.uma.jmetal.operator SelectionOperator

.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: org.uma.jmetal.util SolutionListUtils

.. java:import:: org.uma.jmetal.util SolutionUtils

.. java:import:: org.uma.jmetal.util.comparator DominanceComparator

.. java:import:: java.util Comparator

.. java:import:: java.util List

TournamentSelection
===================

.. java:package:: org.uma.jmetal.operator.impl.selection
   :noindex:

.. java:type:: @SuppressWarnings public class TournamentSelection<S extends Solution<?>> implements SelectionOperator<List<S>, S>

   :author: Juanjo

Constructors
------------
TournamentSelection
^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public TournamentSelection(int numberOfTournaments)
   :outertype: TournamentSelection

   Constructor

TournamentSelection
^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public TournamentSelection(Comparator<S> comparator, int numberOfTournaments)
   :outertype: TournamentSelection

   Constructor

Methods
-------
execute
^^^^^^^

.. java:method:: @Override public S execute(List<S> solutionList)
   :outertype: TournamentSelection

