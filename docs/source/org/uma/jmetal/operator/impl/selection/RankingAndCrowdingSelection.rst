.. java:import:: org.uma.jmetal.operator SelectionOperator

.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: org.uma.jmetal.util.comparator CrowdingDistanceComparator

.. java:import:: org.uma.jmetal.util.comparator DominanceComparator

.. java:import:: org.uma.jmetal.util.solutionattribute Ranking

.. java:import:: org.uma.jmetal.util.solutionattribute.impl CrowdingDistance

.. java:import:: org.uma.jmetal.util.solutionattribute.impl DominanceRanking

.. java:import:: java.util ArrayList

.. java:import:: java.util Collections

.. java:import:: java.util Comparator

.. java:import:: java.util List

RankingAndCrowdingSelection
===========================

.. java:package:: org.uma.jmetal.operator.impl.selection
   :noindex:

.. java:type:: @SuppressWarnings public class RankingAndCrowdingSelection<S extends Solution<?>> implements SelectionOperator<List<S>, List<S>>

   This class implements a selection for selecting a number of solutions from a solution list. The solutions are taken by mean of its ranking and crowding distance values.

   :author: Antonio J. Nebro, Juan J. Durillo

Constructors
------------
RankingAndCrowdingSelection
^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public RankingAndCrowdingSelection(int solutionsToSelect, Comparator<S> dominanceComparator)
   :outertype: RankingAndCrowdingSelection

   Constructor

RankingAndCrowdingSelection
^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public RankingAndCrowdingSelection(int solutionsToSelect)
   :outertype: RankingAndCrowdingSelection

   Constructor

Methods
-------
addLastRankedSolutionsToPopulation
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: protected void addLastRankedSolutionsToPopulation(Ranking<S> ranking, int rank, List<S> population)
   :outertype: RankingAndCrowdingSelection

addRankedSolutionsToPopulation
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: protected void addRankedSolutionsToPopulation(Ranking<S> ranking, int rank, List<S> population)
   :outertype: RankingAndCrowdingSelection

crowdingDistanceSelection
^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: protected List<S> crowdingDistanceSelection(Ranking<S> ranking)
   :outertype: RankingAndCrowdingSelection

execute
^^^^^^^

.. java:method:: public List<S> execute(List<S> solutionList) throws JMetalException
   :outertype: RankingAndCrowdingSelection

   Execute() method

getNumberOfSolutionsToSelect
^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public int getNumberOfSolutionsToSelect()
   :outertype: RankingAndCrowdingSelection

subfrontFillsIntoThePopulation
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: protected boolean subfrontFillsIntoThePopulation(Ranking<S> ranking, int rank, List<S> population)
   :outertype: RankingAndCrowdingSelection

