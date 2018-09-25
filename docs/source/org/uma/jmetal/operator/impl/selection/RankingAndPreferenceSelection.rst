.. java:import:: org.uma.jmetal.operator SelectionOperator

.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: org.uma.jmetal.util.comparator CrowdingDistanceComparator

.. java:import:: org.uma.jmetal.util.solutionattribute Ranking

.. java:import:: org.uma.jmetal.util.solutionattribute.impl DominanceRanking

.. java:import:: org.uma.jmetal.util.solutionattribute.impl PreferenceDistance

.. java:import:: java.util ArrayList

.. java:import:: java.util Collections

.. java:import:: java.util List

RankingAndPreferenceSelection
=============================

.. java:package:: org.uma.jmetal.operator.impl.selection
   :noindex:

.. java:type:: public class RankingAndPreferenceSelection<S extends Solution<?>> implements SelectionOperator<List<S>, List<S>>

Constructors
------------
RankingAndPreferenceSelection
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public RankingAndPreferenceSelection(int solutionsToSelect, List<Double> interestPoint, double epsilon)
   :outertype: RankingAndPreferenceSelection

   Constructor

Methods
-------
addLastRankedSolutionsToPopulation
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: protected void addLastRankedSolutionsToPopulation(Ranking<S> ranking, int rank, List<S> population)
   :outertype: RankingAndPreferenceSelection

addRankedSolutionsToPopulation
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: protected void addRankedSolutionsToPopulation(Ranking<S> ranking, int rank, List<S> population)
   :outertype: RankingAndPreferenceSelection

execute
^^^^^^^

.. java:method:: @Override public List<S> execute(List<S> solutionList)
   :outertype: RankingAndPreferenceSelection

getNumberOfSolutionsToSelect
^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public int getNumberOfSolutionsToSelect()
   :outertype: RankingAndPreferenceSelection

preferenceDistanceSelection
^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: protected List<S> preferenceDistanceSelection(Ranking<S> ranking, int numberOfObjectives)
   :outertype: RankingAndPreferenceSelection

subfrontFillsIntoThePopulation
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: protected boolean subfrontFillsIntoThePopulation(Ranking<S> ranking, int rank, List<S> population)
   :outertype: RankingAndPreferenceSelection

