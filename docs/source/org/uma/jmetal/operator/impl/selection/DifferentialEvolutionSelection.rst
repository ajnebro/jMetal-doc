.. java:import:: org.uma.jmetal.operator SelectionOperator

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: org.uma.jmetal.util.pseudorandom BoundedRandomGenerator

.. java:import:: org.uma.jmetal.util.pseudorandom JMetalRandom

.. java:import:: java.util ArrayList

.. java:import:: java.util List

DifferentialEvolutionSelection
==============================

.. java:package:: org.uma.jmetal.operator.impl.selection
   :noindex:

.. java:type:: @SuppressWarnings public class DifferentialEvolutionSelection implements SelectionOperator<List<DoubleSolution>, List<DoubleSolution>>

   Class implementing the selection operator used in DE: three different solutions are returned from a population. The three solutions must be also different from the one indicated by an index (its position in the list). As a consequence, the operator requires a solution list with at least for elements.

   :author: Antonio J. Nebro , Juan J. Durillo

Constructors
------------
DifferentialEvolutionSelection
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public DifferentialEvolutionSelection()
   :outertype: DifferentialEvolutionSelection

   Constructor

DifferentialEvolutionSelection
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public DifferentialEvolutionSelection(BoundedRandomGenerator<Integer> randomGenerator)
   :outertype: DifferentialEvolutionSelection

   Constructor

Methods
-------
execute
^^^^^^^

.. java:method:: @Override public List<DoubleSolution> execute(List<DoubleSolution> solutionSet)
   :outertype: DifferentialEvolutionSelection

   Execute() method

setIndex
^^^^^^^^

.. java:method:: public void setIndex(int index)
   :outertype: DifferentialEvolutionSelection

