.. java:import:: org.uma.jmetal.operator SelectionOperator

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: org.uma.jmetal.util SolutionListUtils

.. java:import:: java.util List

NaryRandomSelection
===================

.. java:package:: org.uma.jmetal.operator.impl.selection
   :noindex:

.. java:type:: @SuppressWarnings public class NaryRandomSelection<S> implements SelectionOperator<List<S>, List<S>>

   This class implements a random selection operator used for selecting a N number of solutions from a list

   :author: Antonio J. Nebro

Constructors
------------
NaryRandomSelection
^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public NaryRandomSelection()
   :outertype: NaryRandomSelection

   Constructor

NaryRandomSelection
^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public NaryRandomSelection(int numberOfSolutionsToBeReturned)
   :outertype: NaryRandomSelection

   Constructor

Methods
-------
execute
^^^^^^^

.. java:method:: public List<S> execute(List<S> solutionList)
   :outertype: NaryRandomSelection

   Execute() method

