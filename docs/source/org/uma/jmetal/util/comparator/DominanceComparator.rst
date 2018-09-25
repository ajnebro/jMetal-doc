.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: org.uma.jmetal.util.comparator.impl OverallConstraintViolationComparator

.. java:import:: java.io Serializable

.. java:import:: java.util Comparator

DominanceComparator
===================

.. java:package:: org.uma.jmetal.util.comparator
   :noindex:

.. java:type:: @SuppressWarnings public class DominanceComparator<S extends Solution<?>> implements Comparator<S>, Serializable

   This class implements a solution comparator taking into account the violation constraints

   :author: Antonio J. Nebro

Constructors
------------
DominanceComparator
^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public DominanceComparator()
   :outertype: DominanceComparator

   Constructor

DominanceComparator
^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public DominanceComparator(double epsilon)
   :outertype: DominanceComparator

   Constructor

DominanceComparator
^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public DominanceComparator(ConstraintViolationComparator<S> constraintComparator)
   :outertype: DominanceComparator

   Constructor

DominanceComparator
^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public DominanceComparator(ConstraintViolationComparator<S> constraintComparator, double epsilon)
   :outertype: DominanceComparator

   Constructor

Methods
-------
compare
^^^^^^^

.. java:method:: @Override public int compare(S solution1, S solution2)
   :outertype: DominanceComparator

   Compares two solutions.

   :param solution1: Object representing the first \ ``Solution``\ .
   :param solution2: Object representing the second \ ``Solution``\ .
   :return: -1, or 0, or 1 if solution1 dominates solution2, both are non-dominated, or solution1 is dominated by solution2, respectively.

