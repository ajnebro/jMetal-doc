.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: java.io Serializable

.. java:import:: java.util Comparator

ObjectiveComparator
===================

.. java:package:: org.uma.jmetal.util.comparator
   :noindex:

.. java:type:: @SuppressWarnings public class ObjectiveComparator<S extends Solution<?>> implements Comparator<S>, Serializable

   This class implements a comparator based on a given objective

   :author: Antonio J. Nebro

Constructors
------------
ObjectiveComparator
^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public ObjectiveComparator(int objectiveId)
   :outertype: ObjectiveComparator

   Constructor.

   :param objectiveId: The index of the objective to compare

ObjectiveComparator
^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public ObjectiveComparator(int objectiveId, Ordering order)
   :outertype: ObjectiveComparator

   Comparator.

   :param objectiveId: The index of the objective to compare
   :param order: Ascending or descending order

Methods
-------
compare
^^^^^^^

.. java:method:: @Override public int compare(S solution1, S solution2)
   :outertype: ObjectiveComparator

   Compares two solutions according to a given objective.

   :param solution1: The first solution
   :param solution2: The second solution
   :return: -1, or 0, or 1 if solution1 is less than, equal, or greater than solution2, respectively, according to the established order

