.. java:import:: org.uma.jmetal.operator SelectionOperator

.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util.archive.impl AdaptiveGridArchive

.. java:import:: org.uma.jmetal.util.pseudorandom JMetalRandom

PESA2Selection
==============

.. java:package:: org.uma.jmetal.algorithm.multiobjective.pesa2.util
   :noindex:

.. java:type:: @SuppressWarnings public class PESA2Selection<S extends Solution<?>> implements SelectionOperator<AdaptiveGridArchive<S>, S>

   This class implements a selection operator as the used in the PESA-II algorithm

Constructors
------------
PESA2Selection
^^^^^^^^^^^^^^

.. java:constructor:: public PESA2Selection()
   :outertype: PESA2Selection

Methods
-------
execute
^^^^^^^

.. java:method:: @Override public S execute(AdaptiveGridArchive<S> archive)
   :outertype: PESA2Selection

