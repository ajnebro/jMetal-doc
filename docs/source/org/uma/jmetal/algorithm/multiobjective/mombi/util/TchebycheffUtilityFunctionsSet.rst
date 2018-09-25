.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: java.util ArrayList

.. java:import:: java.util List

TchebycheffUtilityFunctionsSet
==============================

.. java:package:: org.uma.jmetal.algorithm.multiobjective.mombi.util
   :noindex:

.. java:type:: @SuppressWarnings public class TchebycheffUtilityFunctionsSet<S extends Solution<?>> extends AbstractUtilityFunctionsSet<S>

   This class implements a set of utility functions based on the Tchebycheff aggregation approach

   :author: Juan J. Durillo ToDo List: + check the size of nadir and reference points are the correct ones + check that the function that needs to be evaluated is the correct one
   :param <S>:

Constructors
------------
TchebycheffUtilityFunctionsSet
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public TchebycheffUtilityFunctionsSet(String file_path, List<Double> referencePoint)
   :outertype: TchebycheffUtilityFunctionsSet

TchebycheffUtilityFunctionsSet
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public TchebycheffUtilityFunctionsSet(String file_path)
   :outertype: TchebycheffUtilityFunctionsSet

Methods
-------
evaluate
^^^^^^^^

.. java:method:: @Override public Double evaluate(S solution, int vector)
   :outertype: TchebycheffUtilityFunctionsSet

