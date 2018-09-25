.. java:import:: org.uma.jmetal.operator SelectionOperator

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: java.util Comparator

.. java:import:: java.util List

BestSolutionSelection
=====================

.. java:package:: org.uma.jmetal.operator.impl.selection
   :noindex:

.. java:type:: @SuppressWarnings public class BestSolutionSelection<S> implements SelectionOperator<List<S>, S>

   This class implements a selection operator used for selecting the best solution in a list according to a given comparator.

   :author: Antonio J. Nebro

Constructors
------------
BestSolutionSelection
^^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public BestSolutionSelection(Comparator<S> comparator)
   :outertype: BestSolutionSelection

Methods
-------
execute
^^^^^^^

.. java:method:: public S execute(List<S> solutionList)
   :outertype: BestSolutionSelection

   Execute() method

