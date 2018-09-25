.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util.solutionattribute.impl GenericSolutionAttribute

R2Ranking
=========

.. java:package:: org.uma.jmetal.algorithm.multiobjective.mombi.util
   :noindex:

.. java:type:: @SuppressWarnings public class R2Ranking<S extends Solution<?>> extends GenericSolutionAttribute<S, R2SolutionData>

Constructors
------------
R2Ranking
^^^^^^^^^

.. java:constructor:: public R2Ranking(AbstractUtilityFunctionsSet<S> utilityFunctions)
   :outertype: R2Ranking

Methods
-------
computeRanking
^^^^^^^^^^^^^^

.. java:method:: public R2Ranking<S> computeRanking(List<S> population)
   :outertype: R2Ranking

getAttribute
^^^^^^^^^^^^

.. java:method:: @Override public R2SolutionData getAttribute(S solution)
   :outertype: R2Ranking

getAttributeIdentifier
^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public Object getAttributeIdentifier()
   :outertype: R2Ranking

getNumberOfSubfronts
^^^^^^^^^^^^^^^^^^^^

.. java:method:: public int getNumberOfSubfronts()
   :outertype: R2Ranking

getSubfront
^^^^^^^^^^^

.. java:method:: public List<S> getSubfront(int rank)
   :outertype: R2Ranking

getUtilityFunctions
^^^^^^^^^^^^^^^^^^^

.. java:method:: public AbstractUtilityFunctionsSet<S> getUtilityFunctions()
   :outertype: R2Ranking

setAttribute
^^^^^^^^^^^^

.. java:method:: @Override public void setAttribute(S solution, R2SolutionData value)
   :outertype: R2Ranking

