.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util AdaptiveGrid

.. java:import:: org.uma.jmetal.util.comparator DominanceComparator

.. java:import:: java.util Comparator

.. java:import:: java.util Iterator

AdaptiveGridArchive
===================

.. java:package:: org.uma.jmetal.util.archive.impl
   :noindex:

.. java:type:: @SuppressWarnings public class AdaptiveGridArchive<S extends Solution<?>> extends AbstractBoundedArchive<S>

   This class implements an archive (solution list) based on an adaptive grid used in PAES

   :author: Antonio J. Nebro , Juan J. Durillo

Constructors
------------
AdaptiveGridArchive
^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public AdaptiveGridArchive(int maxSize, int bisections, int objectives)
   :outertype: AdaptiveGridArchive

   Constructor.

   :param maxSize: The maximum size of the setArchive
   :param bisections: The maximum number of bi-divisions for the adaptive grid.
   :param objectives: The number of objectives.

Methods
-------
add
^^^

.. java:method:: @Override public boolean add(S solution)
   :outertype: AdaptiveGridArchive

   Adds a \ ``Solution``\  to the setArchive. If the \ ``Solution``\  is dominated by any member of the setArchive then it is discarded. If the \ ``Solution``\  dominates some members of the setArchive, these are removed. If the setArchive is full and the \ ``Solution``\  has to be inserted, one \ ``Solution``\  of the most populated hypercube of the adaptive grid is removed.

   :param solution: The \ ``Solution``\
   :return: true if the \ ``Solution``\  has been inserted, false otherwise.

computeDensityEstimator
^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public void computeDensityEstimator()
   :outertype: AdaptiveGridArchive

getComparator
^^^^^^^^^^^^^

.. java:method:: @Override public Comparator<S> getComparator()
   :outertype: AdaptiveGridArchive

getGrid
^^^^^^^

.. java:method:: public AdaptiveGrid<S> getGrid()
   :outertype: AdaptiveGridArchive

prune
^^^^^

.. java:method:: public void prune()
   :outertype: AdaptiveGridArchive

sortByDensityEstimator
^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public void sortByDensityEstimator()
   :outertype: AdaptiveGridArchive

