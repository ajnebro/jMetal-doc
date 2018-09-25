.. java:import:: org.apache.commons.lang3.tuple Pair

.. java:import:: org.uma.jmetal.operator SelectionOperator

.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util SolutionListUtils

.. java:import:: org.uma.jmetal.util.comparator StrengthFitnessComparator

.. java:import:: org.uma.jmetal.util.solutionattribute.impl LocationAttribute

.. java:import:: org.uma.jmetal.util.solutionattribute.impl StrengthRawFitness

EnvironmentalSelection
======================

.. java:package:: org.uma.jmetal.algorithm.multiobjective.spea2.util
   :noindex:

.. java:type:: @SuppressWarnings public class EnvironmentalSelection<S extends Solution<?>> implements SelectionOperator<List<S>, List<S>>

   :author: Juanjo Durillo
   :param <S>:

Constructors
------------
EnvironmentalSelection
^^^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public EnvironmentalSelection(int solutionsToSelect)
   :outertype: EnvironmentalSelection

Methods
-------
execute
^^^^^^^

.. java:method:: @Override public List<S> execute(List<S> source2)
   :outertype: EnvironmentalSelection

