.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: java.util ArrayList

.. java:import:: java.util List

PreferenceNSGAII
================

.. java:package:: org.uma.jmetal.algorithm.multiobjective.rnsgaii.util
   :noindex:

.. java:type:: public class PreferenceNSGAII<S extends Solution<?>>

Constructors
------------
PreferenceNSGAII
^^^^^^^^^^^^^^^^

.. java:constructor:: public PreferenceNSGAII(List<Double> weights)
   :outertype: PreferenceNSGAII

Methods
-------
evaluate
^^^^^^^^

.. java:method:: public Double evaluate(S solution)
   :outertype: PreferenceNSGAII

getSize
^^^^^^^

.. java:method:: public int getSize()
   :outertype: PreferenceNSGAII

setLowerBounds
^^^^^^^^^^^^^^

.. java:method:: public void setLowerBounds(List<Double> lowerBounds)
   :outertype: PreferenceNSGAII

setUpperBounds
^^^^^^^^^^^^^^

.. java:method:: public void setUpperBounds(List<Double> upperBounds)
   :outertype: PreferenceNSGAII

updatePointOfInterest
^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public void updatePointOfInterest(List<Double> newInterestPoint)
   :outertype: PreferenceNSGAII

