.. java:import:: org.uma.jmetal.solution Solution

R2RankingNormalized
===================

.. java:package:: org.uma.jmetal.algorithm.multiobjective.mombi.util
   :noindex:

.. java:type:: @SuppressWarnings public class R2RankingNormalized<S extends Solution<?>> extends R2Ranking<S>

Constructors
------------
R2RankingNormalized
^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public R2RankingNormalized(AbstractUtilityFunctionsSet<S> utilityFunctions, Normalizer normalizer)
   :outertype: R2RankingNormalized

Methods
-------
computeRanking
^^^^^^^^^^^^^^

.. java:method:: public R2RankingNormalized<S> computeRanking(List<S> population)
   :outertype: R2RankingNormalized

getNumberOfSubfronts
^^^^^^^^^^^^^^^^^^^^

.. java:method:: public int getNumberOfSubfronts()
   :outertype: R2RankingNormalized

getSubfront
^^^^^^^^^^^

.. java:method:: public List<S> getSubfront(int rank)
   :outertype: R2RankingNormalized

