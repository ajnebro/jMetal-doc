.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util.comparator ConstraintViolationComparator

.. java:import:: org.uma.jmetal.util.solutionattribute.impl OverallConstraintViolation

OverallConstraintViolationComparator
====================================

.. java:package:: org.uma.jmetal.util.comparator.impl
   :noindex:

.. java:type:: @SuppressWarnings public class OverallConstraintViolationComparator<S extends Solution<?>> implements ConstraintViolationComparator<S>

   This class implements a \ ``Comparator``\  (a method for comparing \ ``Solution``\  objects) based on the overall constraint violation of the solutions, as done in NSGA-II.

   :author: Antonio J. Nebro

Constructors
------------
OverallConstraintViolationComparator
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public OverallConstraintViolationComparator()
   :outertype: OverallConstraintViolationComparator

   Constructor

Methods
-------
compare
^^^^^^^

.. java:method:: public int compare(S solution1, S solution2)
   :outertype: OverallConstraintViolationComparator

   Compares two solutions. If the solutions has no constraints the method return 0

   :param solution1: Object representing the first \ ``Solution``\ .
   :param solution2: Object representing the second \ ``Solution``\ .
   :return: -1, or 0, or 1 if o1 is less than, equal, or greater than o2, respectively.

