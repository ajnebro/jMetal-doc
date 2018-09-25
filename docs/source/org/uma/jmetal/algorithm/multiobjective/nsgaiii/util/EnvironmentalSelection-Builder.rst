.. java:import:: org.uma.jmetal.operator SelectionOperator

.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: org.uma.jmetal.util.pseudorandom JMetalRandom

.. java:import:: org.uma.jmetal.util.solutionattribute SolutionAttribute

.. java:import:: java.util ArrayList

.. java:import:: java.util List

EnvironmentalSelection.Builder
==============================

.. java:package:: org.uma.jmetal.algorithm.multiobjective.nsgaiii.util
   :noindex:

.. java:type:: public static class Builder<S extends Solution<?>>
   :outertype: EnvironmentalSelection

Methods
-------
build
^^^^^

.. java:method:: public EnvironmentalSelection<S> build()
   :outertype: EnvironmentalSelection.Builder

getFronts
^^^^^^^^^

.. java:method:: public List<List<S>> getFronts()
   :outertype: EnvironmentalSelection.Builder

getNumberOfObjectives
^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public int getNumberOfObjectives()
   :outertype: EnvironmentalSelection.Builder

getReferencePoints
^^^^^^^^^^^^^^^^^^

.. java:method:: public List<ReferencePoint<S>> getReferencePoints()
   :outertype: EnvironmentalSelection.Builder

getSolutionsToSelet
^^^^^^^^^^^^^^^^^^^

.. java:method:: public int getSolutionsToSelet()
   :outertype: EnvironmentalSelection.Builder

setFronts
^^^^^^^^^

.. java:method:: public Builder<S> setFronts(List<List<S>> f)
   :outertype: EnvironmentalSelection.Builder

setNumberOfObjectives
^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public Builder<S> setNumberOfObjectives(int n)
   :outertype: EnvironmentalSelection.Builder

setReferencePoints
^^^^^^^^^^^^^^^^^^

.. java:method:: public Builder<S> setReferencePoints(List<ReferencePoint<S>> referencePoints)
   :outertype: EnvironmentalSelection.Builder

setSolutionsToSelect
^^^^^^^^^^^^^^^^^^^^

.. java:method:: public Builder<S> setSolutionsToSelect(int solutions)
   :outertype: EnvironmentalSelection.Builder

