.. java:import:: org.uma.jmetal.problem.impl AbstractBinaryProblem

.. java:import:: org.uma.jmetal.solution BinarySolution

.. java:import:: org.uma.jmetal.solution.impl DefaultBinarySolution

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: java.util BitSet

OneMax
======

.. java:package:: org.uma.jmetal.problem.singleobjective
   :noindex:

.. java:type:: @SuppressWarnings public class OneMax extends AbstractBinaryProblem

   Class representing problem OneMax. The problem consist of maximizing the number of '1's in a binary string.

Constructors
------------
OneMax
^^^^^^

.. java:constructor:: public OneMax()
   :outertype: OneMax

   Constructor

OneMax
^^^^^^

.. java:constructor:: public OneMax(Integer numberOfBits)
   :outertype: OneMax

   Constructor

Methods
-------
createSolution
^^^^^^^^^^^^^^

.. java:method:: @Override public BinarySolution createSolution()
   :outertype: OneMax

evaluate
^^^^^^^^

.. java:method:: @Override public void evaluate(BinarySolution solution)
   :outertype: OneMax

   Evaluate() method

getBitsPerVariable
^^^^^^^^^^^^^^^^^^

.. java:method:: @Override protected int getBitsPerVariable(int index)
   :outertype: OneMax

