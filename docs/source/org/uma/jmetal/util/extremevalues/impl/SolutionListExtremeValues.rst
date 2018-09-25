.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util.extremevalues ExtremeValuesFinder

.. java:import:: org.uma.jmetal.util.front.imp ArrayFront

.. java:import:: java.util List

SolutionListExtremeValues
=========================

.. java:package:: org.uma.jmetal.util.extremevalues.impl
   :noindex:

.. java:type:: public class SolutionListExtremeValues implements ExtremeValuesFinder<List<Solution<?>>, List<Double>>

   Class for finding the extreme values of a list of objects

   :author: Antonio J. Nebro

Methods
-------
findHighestValues
^^^^^^^^^^^^^^^^^

.. java:method:: @Override public List<Double> findHighestValues(List<Solution<?>> solutionList)
   :outertype: SolutionListExtremeValues

findLowestValues
^^^^^^^^^^^^^^^^

.. java:method:: @Override public List<Double> findLowestValues(List<Solution<?>> solutionList)
   :outertype: SolutionListExtremeValues

