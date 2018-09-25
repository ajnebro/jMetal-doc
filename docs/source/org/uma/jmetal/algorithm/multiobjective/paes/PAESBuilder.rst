.. java:import:: org.uma.jmetal.operator MutationOperator

.. java:import:: org.uma.jmetal.problem Problem

.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util AlgorithmBuilder

PAESBuilder
===========

.. java:package:: org.uma.jmetal.algorithm.multiobjective.paes
   :noindex:

.. java:type:: public class PAESBuilder<S extends Solution<?>> implements AlgorithmBuilder<PAES<S>>

   :author: Antonio J. Nebro

Constructors
------------
PAESBuilder
^^^^^^^^^^^

.. java:constructor:: public PAESBuilder(Problem<S> problem)
   :outertype: PAESBuilder

Methods
-------
build
^^^^^

.. java:method:: public PAES<S> build()
   :outertype: PAESBuilder

getArchiveSize
^^^^^^^^^^^^^^

.. java:method:: public int getArchiveSize()
   :outertype: PAESBuilder

getBiSections
^^^^^^^^^^^^^

.. java:method:: public int getBiSections()
   :outertype: PAESBuilder

getMaxEvaluations
^^^^^^^^^^^^^^^^^

.. java:method:: public int getMaxEvaluations()
   :outertype: PAESBuilder

getMutationOperator
^^^^^^^^^^^^^^^^^^^

.. java:method:: public MutationOperator<S> getMutationOperator()
   :outertype: PAESBuilder

getProblem
^^^^^^^^^^

.. java:method:: public Problem<S> getProblem()
   :outertype: PAESBuilder

setArchiveSize
^^^^^^^^^^^^^^

.. java:method:: public PAESBuilder<S> setArchiveSize(int archiveSize)
   :outertype: PAESBuilder

setBiSections
^^^^^^^^^^^^^

.. java:method:: public PAESBuilder<S> setBiSections(int biSections)
   :outertype: PAESBuilder

setMaxEvaluations
^^^^^^^^^^^^^^^^^

.. java:method:: public PAESBuilder<S> setMaxEvaluations(int maxEvaluations)
   :outertype: PAESBuilder

setMutationOperator
^^^^^^^^^^^^^^^^^^^

.. java:method:: public PAESBuilder<S> setMutationOperator(MutationOperator<S> mutation)
   :outertype: PAESBuilder

