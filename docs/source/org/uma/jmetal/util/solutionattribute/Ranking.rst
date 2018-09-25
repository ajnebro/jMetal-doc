.. java:import:: java.util List

Ranking
=======

.. java:package:: org.uma.jmetal.util.solutionattribute
   :noindex:

.. java:type:: public interface Ranking<S> extends SolutionAttribute<S, Integer>

   Ranks a list of solutions according to the dominance relationship

   :author: Antonio J. Nebro

Methods
-------
computeRanking
^^^^^^^^^^^^^^

.. java:method:: public Ranking<S> computeRanking(List<S> solutionList)
   :outertype: Ranking

getNumberOfSubfronts
^^^^^^^^^^^^^^^^^^^^

.. java:method:: public int getNumberOfSubfronts()
   :outertype: Ranking

getSubfront
^^^^^^^^^^^

.. java:method:: public List<S> getSubfront(int rank)
   :outertype: Ranking

