.. java:import:: org.uma.jmetal.problem PermutationProblem

.. java:import:: org.uma.jmetal.solution PermutationSolution

.. java:import:: java.util ArrayList

.. java:import:: java.util HashMap

.. java:import:: java.util List

DefaultIntegerPermutationSolution
=================================

.. java:package:: org.uma.jmetal.solution.impl
   :noindex:

.. java:type:: @SuppressWarnings public class DefaultIntegerPermutationSolution extends AbstractGenericSolution<Integer, PermutationProblem<?>> implements PermutationSolution<Integer>

   Defines an implementation of solution composed of a permuation of integers

   :author: Antonio J. Nebro

Constructors
------------
DefaultIntegerPermutationSolution
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public DefaultIntegerPermutationSolution(PermutationProblem<?> problem)
   :outertype: DefaultIntegerPermutationSolution

   Constructor

DefaultIntegerPermutationSolution
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public DefaultIntegerPermutationSolution(DefaultIntegerPermutationSolution solution)
   :outertype: DefaultIntegerPermutationSolution

   Copy Constructor

Methods
-------
copy
^^^^

.. java:method:: @Override public DefaultIntegerPermutationSolution copy()
   :outertype: DefaultIntegerPermutationSolution

getVariableValueString
^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public String getVariableValueString(int index)
   :outertype: DefaultIntegerPermutationSolution

