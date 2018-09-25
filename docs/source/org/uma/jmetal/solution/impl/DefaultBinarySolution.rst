.. java:import:: org.uma.jmetal.problem BinaryProblem

.. java:import:: org.uma.jmetal.solution BinarySolution

.. java:import:: org.uma.jmetal.util.binarySet BinarySet

.. java:import:: java.util HashMap

DefaultBinarySolution
=====================

.. java:package:: org.uma.jmetal.solution.impl
   :noindex:

.. java:type:: @SuppressWarnings public class DefaultBinarySolution extends AbstractGenericSolution<BinarySet, BinaryProblem> implements BinarySolution

   Defines an implementation of a binary solution

   :author: Antonio J. Nebro

Constructors
------------
DefaultBinarySolution
^^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public DefaultBinarySolution(BinaryProblem problem)
   :outertype: DefaultBinarySolution

   Constructor

DefaultBinarySolution
^^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public DefaultBinarySolution(DefaultBinarySolution solution)
   :outertype: DefaultBinarySolution

   Copy constructor

Methods
-------
copy
^^^^

.. java:method:: @Override public DefaultBinarySolution copy()
   :outertype: DefaultBinarySolution

getNumberOfBits
^^^^^^^^^^^^^^^

.. java:method:: @Override public int getNumberOfBits(int index)
   :outertype: DefaultBinarySolution

getTotalNumberOfBits
^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public int getTotalNumberOfBits()
   :outertype: DefaultBinarySolution

getVariableValueString
^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public String getVariableValueString(int index)
   :outertype: DefaultBinarySolution

