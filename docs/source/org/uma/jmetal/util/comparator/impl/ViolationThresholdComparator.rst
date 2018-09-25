.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util.comparator ConstraintViolationComparator

.. java:import:: org.uma.jmetal.util.solutionattribute.impl NumberOfViolatedConstraints

.. java:import:: org.uma.jmetal.util.solutionattribute.impl OverallConstraintViolation

.. java:import:: java.util List

ViolationThresholdComparator
============================

.. java:package:: org.uma.jmetal.util.comparator.impl
   :noindex:

.. java:type:: @SuppressWarnings public class ViolationThresholdComparator<S extends Solution<?>> implements ConstraintViolationComparator<S>

   This class implements the ViolationThreshold Comparator *

   :author: Juan J. Durillo

Constructors
------------
ViolationThresholdComparator
^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public ViolationThresholdComparator()
   :outertype: ViolationThresholdComparator

   Constructor

Methods
-------
compare
^^^^^^^

.. java:method:: @Override public int compare(S solution1, S solution2)
   :outertype: ViolationThresholdComparator

   Compares two solutions. If the solutions has no constraints the method return 0

   :param solution1: Object representing the first \ ``Solution``\ .
   :param solution2: Object representing the second \ ``Solution``\ .
   :return: -1, or 0, or 1 if o1 is less than, equal, or greater than o2, respectively.

feasibilityRatio
^^^^^^^^^^^^^^^^

.. java:method:: public double feasibilityRatio(List<S> solutionSet)
   :outertype: ViolationThresholdComparator

   Computes the feasibility ratio Return the ratio of feasible solutions

meanOverallViolation
^^^^^^^^^^^^^^^^^^^^

.. java:method:: public double meanOverallViolation(List<S> solutionSet)
   :outertype: ViolationThresholdComparator

   Computes the feasibility ratio Return the ratio of feasible solutions

needToCompare
^^^^^^^^^^^^^

.. java:method:: public boolean needToCompare(S solution1, S solution2)
   :outertype: ViolationThresholdComparator

   Returns true if solutions s1 and/or s2 have an overall constraint violation with value less than 0

updateThreshold
^^^^^^^^^^^^^^^

.. java:method:: public void updateThreshold(List<S> set)
   :outertype: ViolationThresholdComparator

   Updates the threshold value using the population

