.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: java.util ArrayList

.. java:import:: java.util List

ASFUtilityFunctionSet
=====================

.. java:package:: org.uma.jmetal.algorithm.multiobjective.mombi.util
   :noindex:

.. java:type:: @SuppressWarnings public class ASFUtilityFunctionSet<S extends Solution<?>> extends AbstractUtilityFunctionsSet<S>

   :author: Juan J. Durillo Modified by Antonio J. Nebro
   :param <S>:

Constructors
------------
ASFUtilityFunctionSet
^^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public ASFUtilityFunctionSet(double[][] weights, List<Double> referencePoint)
   :outertype: ASFUtilityFunctionSet

ASFUtilityFunctionSet
^^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public ASFUtilityFunctionSet(double[][] weights)
   :outertype: ASFUtilityFunctionSet

ASFUtilityFunctionSet
^^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public ASFUtilityFunctionSet(String file_path, List<Double> referencePoint)
   :outertype: ASFUtilityFunctionSet

ASFUtilityFunctionSet
^^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public ASFUtilityFunctionSet(String file_path)
   :outertype: ASFUtilityFunctionSet

Methods
-------
evaluate
^^^^^^^^

.. java:method:: @Override public Double evaluate(S solution, int vector)
   :outertype: ASFUtilityFunctionSet

setNormalizer
^^^^^^^^^^^^^

.. java:method:: public void setNormalizer(Normalizer normalizer)
   :outertype: ASFUtilityFunctionSet

