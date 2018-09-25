.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util SolutionListUtils

.. java:import:: org.uma.jmetal.util.comparator DominanceComparator

.. java:import:: org.uma.jmetal.util.solutionattribute DensityEstimator

.. java:import:: java.util Arrays

.. java:import:: java.util Comparator

.. java:import:: java.util List

StrengthRawFitness
==================

.. java:package:: org.uma.jmetal.util.solutionattribute.impl
   :noindex:

.. java:type:: @SuppressWarnings public class StrengthRawFitness<S extends Solution<?>> extends GenericSolutionAttribute<S, Double> implements DensityEstimator<S>

Methods
-------
computeDensityEstimator
^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public void computeDensityEstimator(List<S> solutionSet)
   :outertype: StrengthRawFitness

