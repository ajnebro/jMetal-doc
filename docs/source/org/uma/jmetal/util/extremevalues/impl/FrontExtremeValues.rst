.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: org.uma.jmetal.util.extremevalues ExtremeValuesFinder

.. java:import:: org.uma.jmetal.util.front Front

.. java:import:: java.util ArrayList

.. java:import:: java.util List

FrontExtremeValues
==================

.. java:package:: org.uma.jmetal.util.extremevalues.impl
   :noindex:

.. java:type:: public class FrontExtremeValues implements ExtremeValuesFinder<Front, List<Double>>

   Class for finding the extreme values of front objects

   :author: Antonio J. Nebro

Methods
-------
findHighestValues
^^^^^^^^^^^^^^^^^

.. java:method:: @Override public List<Double> findHighestValues(Front front)
   :outertype: FrontExtremeValues

findLowestValues
^^^^^^^^^^^^^^^^

.. java:method:: @Override public List<Double> findLowestValues(Front front)
   :outertype: FrontExtremeValues

