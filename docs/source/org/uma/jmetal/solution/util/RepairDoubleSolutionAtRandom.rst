.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: org.uma.jmetal.util.pseudorandom BoundedRandomGenerator

.. java:import:: org.uma.jmetal.util.pseudorandom JMetalRandom

RepairDoubleSolutionAtRandom
============================

.. java:package:: org.uma.jmetal.solution.util
   :noindex:

.. java:type:: @SuppressWarnings public class RepairDoubleSolutionAtRandom implements RepairDoubleSolution

   :author: Antonio J. Nebro

Constructors
------------
RepairDoubleSolutionAtRandom
^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public RepairDoubleSolutionAtRandom()
   :outertype: RepairDoubleSolutionAtRandom

   Constructor

RepairDoubleSolutionAtRandom
^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public RepairDoubleSolutionAtRandom(BoundedRandomGenerator<Double> randomGenerator)
   :outertype: RepairDoubleSolutionAtRandom

   Constructor

Methods
-------
repairSolutionVariableValue
^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public double repairSolutionVariableValue(double value, double lowerBound, double upperBound)
   :outertype: RepairDoubleSolutionAtRandom

   Checks if the value is between its bounds; if not, a random value between the limits is returned

   :param value: The value to be checked
   :param lowerBound:
   :param upperBound:
   :return: The same value if it is between the limits or a repaired value otherwise

