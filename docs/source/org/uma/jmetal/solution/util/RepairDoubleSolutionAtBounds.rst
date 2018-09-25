.. java:import:: org.uma.jmetal.util JMetalException

RepairDoubleSolutionAtBounds
============================

.. java:package:: org.uma.jmetal.solution.util
   :noindex:

.. java:type:: @SuppressWarnings public class RepairDoubleSolutionAtBounds implements RepairDoubleSolution

   :author: Antonio J. Nebro

Methods
-------
repairSolutionVariableValue
^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public double repairSolutionVariableValue(double value, double lowerBound, double upperBound)
   :outertype: RepairDoubleSolutionAtBounds

   Checks if the value is between its bounds; if not, the lower or upper bound is returned

   :param value: The value to be checked
   :param lowerBound:
   :param upperBound:
   :return: The same value if it is in the limits or a repaired value otherwise

