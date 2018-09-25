.. java:import:: org.uma.jmetal.problem BinaryProblem

.. java:import:: org.uma.jmetal.solution BinarySolution

.. java:import:: org.uma.jmetal.solution.impl DefaultBinarySolution

AbstractBinaryProblem
=====================

.. java:package:: org.uma.jmetal.problem.impl
   :noindex:

.. java:type:: @SuppressWarnings public abstract class AbstractBinaryProblem extends AbstractGenericProblem<BinarySolution> implements BinaryProblem

Methods
-------
createSolution
^^^^^^^^^^^^^^

.. java:method:: @Override public BinarySolution createSolution()
   :outertype: AbstractBinaryProblem

getBitsPerVariable
^^^^^^^^^^^^^^^^^^

.. java:method:: protected abstract int getBitsPerVariable(int index)
   :outertype: AbstractBinaryProblem

getNumberOfBits
^^^^^^^^^^^^^^^

.. java:method:: @Override public int getNumberOfBits(int index)
   :outertype: AbstractBinaryProblem

getTotalNumberOfBits
^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public int getTotalNumberOfBits()
   :outertype: AbstractBinaryProblem

