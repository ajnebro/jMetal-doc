.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: org.uma.jmetal.util.comparator DominanceComparator

.. java:import:: org.uma.jmetal.util.comparator.impl OverallConstraintViolationComparator

.. java:import:: org.uma.jmetal.util.solutionattribute Ranking

DominanceRanking
================

.. java:package:: org.uma.jmetal.util.solutionattribute.impl
   :noindex:

.. java:type:: @SuppressWarnings public class DominanceRanking<S extends Solution<?>> extends GenericSolutionAttribute<S, Integer> implements Ranking<S>

   This class implements some facilities for ranking set of solutions. Given a collection of solutions, they are ranked according to scheme proposed in NSGA-II; as an output, a set of subsets are obtained. The subsets are numbered starting from 0 (in NSGA-II, the numbering starts from 1); thus, subset 0 contains the non-dominated solutions, subset 1 contains the non-dominated solutions after removing those belonging to subset 0, and so on.

   :author: Antonio J. Nebro , Juan J. Durillo

Constructors
------------
DominanceRanking
^^^^^^^^^^^^^^^^

.. java:constructor:: public DominanceRanking(Comparator<S> comparator)
   :outertype: DominanceRanking

   Constructor

DominanceRanking
^^^^^^^^^^^^^^^^

.. java:constructor:: public DominanceRanking()
   :outertype: DominanceRanking

   Constructor

DominanceRanking
^^^^^^^^^^^^^^^^

.. java:constructor:: public DominanceRanking(Object id)
   :outertype: DominanceRanking

Methods
-------
computeRanking
^^^^^^^^^^^^^^

.. java:method:: @Override public Ranking<S> computeRanking(List<S> solutionSet)
   :outertype: DominanceRanking

getNumberOfSubfronts
^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public int getNumberOfSubfronts()
   :outertype: DominanceRanking

getSubfront
^^^^^^^^^^^

.. java:method:: @Override public List<S> getSubfront(int rank)
   :outertype: DominanceRanking

