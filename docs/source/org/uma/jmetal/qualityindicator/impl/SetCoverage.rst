.. java:import:: org.apache.commons.lang3.tuple ImmutablePair

.. java:import:: org.apache.commons.lang3.tuple Pair

.. java:import:: org.uma.jmetal.qualityindicator QualityIndicator

.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: org.uma.jmetal.util SolutionListUtils

.. java:import:: org.uma.jmetal.util.naming.impl SimpleDescribedEntity

.. java:import:: java.util List

SetCoverage
===========

.. java:package:: org.uma.jmetal.qualityindicator.impl
   :noindex:

.. java:type:: @SuppressWarnings public class SetCoverage extends SimpleDescribedEntity implements QualityIndicator<Pair<List<? extends Solution<?>>, List<? extends Solution<?>>>, Pair<Double, Double>>

   Set coverage metric

   :author: Antonio J. Nebro

Constructors
------------
SetCoverage
^^^^^^^^^^^

.. java:constructor:: public SetCoverage()
   :outertype: SetCoverage

   Constructor

Methods
-------
evaluate
^^^^^^^^

.. java:method:: @Override public Pair<Double, Double> evaluate(Pair<List<? extends Solution<?>>, List<? extends Solution<?>>> pairOfSolutionLists)
   :outertype: SetCoverage

evaluate
^^^^^^^^

.. java:method:: public double evaluate(List<? extends Solution<?>> set1, List<? extends Solution<?>> set2)
   :outertype: SetCoverage

   Calculates the set coverage of set1 over set2

   :param set1:
   :param set2:
   :return: The value of the set coverage

getName
^^^^^^^

.. java:method:: @Override public String getName()
   :outertype: SetCoverage

