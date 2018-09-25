.. java:import:: org.uma.jmetal.problem.impl AbstractBinaryProblem

.. java:import:: org.uma.jmetal.solution BinarySolution

.. java:import:: org.uma.jmetal.solution.impl DefaultBinarySolution

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: java.util BitSet

OneZeroMax
==========

.. java:package:: org.uma.jmetal.problem.multiobjective
   :noindex:

.. java:type:: @SuppressWarnings public class OneZeroMax extends AbstractBinaryProblem

   Class representing problem OneZeroMax. The problem consist of maximizing the number of '1's and '0's in a binary string.

Constructors
------------
OneZeroMax
^^^^^^^^^^

.. java:constructor:: public OneZeroMax() throws JMetalException
   :outertype: OneZeroMax

   Constructor

OneZeroMax
^^^^^^^^^^

.. java:constructor:: public OneZeroMax(Integer numberOfBits) throws JMetalException
   :outertype: OneZeroMax

   Constructor

Methods
-------
createSolution
^^^^^^^^^^^^^^

.. java:method:: @Override public BinarySolution createSolution()
   :outertype: OneZeroMax

evaluate
^^^^^^^^

.. java:method:: @Override public void evaluate(BinarySolution solution)
   :outertype: OneZeroMax

   Evaluate() method

getBitsPerVariable
^^^^^^^^^^^^^^^^^^

.. java:method:: @Override protected int getBitsPerVariable(int index)
   :outertype: OneZeroMax

