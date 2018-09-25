.. java:import:: java.io Serializable

RepairDoubleSolution
====================

.. java:package:: org.uma.jmetal.solution.util
   :noindex:

.. java:type:: public interface RepairDoubleSolution extends Serializable

   :author: Antonio J. Nebro

Methods
-------
repairSolutionVariableValue
^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public double repairSolutionVariableValue(double value, double lowerBound, double upperBound)
   :outertype: RepairDoubleSolution

   Checks if a given value is between its bounds and repairs it otherwise

   :param value: The value to be checked
   :param lowerBound:
   :param upperBound:
   :return: The same value if it is between the limits or a repaired value otherwise

