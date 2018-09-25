.. java:import:: org.uma.jmetal.operator SelectionOperator

.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: org.uma.jmetal.util.pseudorandom JMetalRandom

.. java:import:: org.uma.jmetal.util.solutionattribute SolutionAttribute

.. java:import:: java.util ArrayList

.. java:import:: java.util List

EnvironmentalSelection
======================

.. java:package:: org.uma.jmetal.algorithm.multiobjective.nsgaiii.util
   :noindex:

.. java:type:: @SuppressWarnings public class EnvironmentalSelection<S extends Solution<?>> implements SelectionOperator<List<S>, List<S>>, SolutionAttribute<S, List<Double>>

Constructors
------------
EnvironmentalSelection
^^^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public EnvironmentalSelection(Builder<S> builder)
   :outertype: EnvironmentalSelection

EnvironmentalSelection
^^^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public EnvironmentalSelection(List<List<S>> fronts, int solutionsToSelect, List<ReferencePoint<S>> referencePoints, int numberOfObjectives)
   :outertype: EnvironmentalSelection

Methods
-------
FindNicheReferencePoint
^^^^^^^^^^^^^^^^^^^^^^^

.. java:method::  int FindNicheReferencePoint()
   :outertype: EnvironmentalSelection

SelectClusterMember
^^^^^^^^^^^^^^^^^^^

.. java:method::  S SelectClusterMember(ReferencePoint<S> rp)
   :outertype: EnvironmentalSelection

associate
^^^^^^^^^

.. java:method:: public void associate(List<S> population)
   :outertype: EnvironmentalSelection

constructHyperplane
^^^^^^^^^^^^^^^^^^^

.. java:method:: public List<Double> constructHyperplane(List<S> population, List<S> extreme_points)
   :outertype: EnvironmentalSelection

execute
^^^^^^^

.. java:method:: @Override public List<S> execute(List<S> source) throws JMetalException
   :outertype: EnvironmentalSelection

getAttribute
^^^^^^^^^^^^

.. java:method:: @Override @SuppressWarnings public List<Double> getAttribute(S solution)
   :outertype: EnvironmentalSelection

getAttributeIdentifier
^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public Object getAttributeIdentifier()
   :outertype: EnvironmentalSelection

guassianElimination
^^^^^^^^^^^^^^^^^^^

.. java:method:: public List<Double> guassianElimination(List<List<Double>> A, List<Double> b)
   :outertype: EnvironmentalSelection

normalizeObjectives
^^^^^^^^^^^^^^^^^^^

.. java:method:: public void normalizeObjectives(List<S> population, List<Double> intercepts, List<Double> ideal_point)
   :outertype: EnvironmentalSelection

perpendicularDistance
^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public double perpendicularDistance(List<Double> direction, List<Double> point)
   :outertype: EnvironmentalSelection

setAttribute
^^^^^^^^^^^^

.. java:method:: @Override public void setAttribute(S solution, List<Double> value)
   :outertype: EnvironmentalSelection

translateObjectives
^^^^^^^^^^^^^^^^^^^

.. java:method:: public List<Double> translateObjectives(List<S> population)
   :outertype: EnvironmentalSelection

