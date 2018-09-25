.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: java.util List

ScalarizationWrapper.ScalarizationType
======================================

.. java:package:: org.uma.jmetal.algorithm.multiobjective.espea.util
   :noindex:

.. java:type:: public static enum ScalarizationType
   :outertype: ScalarizationWrapper

   The scalarization function that is used for computing values.

   :author: Marlon Braun

Enum Constants
--------------
ANGLE_UTILITY
^^^^^^^^^^^^^

.. java:field:: public static final ScalarizationWrapper.ScalarizationType ANGLE_UTILITY
   :outertype: ScalarizationWrapper.ScalarizationType

   Scalarization values are based on maximum angles to extreme points (see "Angle based Preferences Models in Multi-objective Optimization" by Braun et al.)

CHEBYSHEV
^^^^^^^^^

.. java:field:: public static final ScalarizationWrapper.ScalarizationType CHEBYSHEV
   :outertype: ScalarizationWrapper.ScalarizationType

   Chebyhsev scalarization function.

NASH
^^^^

.. java:field:: public static final ScalarizationWrapper.ScalarizationType NASH
   :outertype: ScalarizationWrapper.ScalarizationType

   The Nash bargaining solution

PRODUCT_OF_OBJECTIVES
^^^^^^^^^^^^^^^^^^^^^

.. java:field:: public static final ScalarizationWrapper.ScalarizationType PRODUCT_OF_OBJECTIVES
   :outertype: ScalarizationWrapper.ScalarizationType

   Multiplication of all objectives.

SUM_OF_OBJECTIVES
^^^^^^^^^^^^^^^^^

.. java:field:: public static final ScalarizationWrapper.ScalarizationType SUM_OF_OBJECTIVES
   :outertype: ScalarizationWrapper.ScalarizationType

   Summing up all objectives.

TRADEOFF_UTILITY
^^^^^^^^^^^^^^^^

.. java:field:: public static final ScalarizationWrapper.ScalarizationType TRADEOFF_UTILITY
   :outertype: ScalarizationWrapper.ScalarizationType

   Tradeoff utility also known as proper utility (see "Theory and Algorithms for Finding Knees" by Shukla et al.).

UNIFORM
^^^^^^^

.. java:field:: public static final ScalarizationWrapper.ScalarizationType UNIFORM
   :outertype: ScalarizationWrapper.ScalarizationType

   All solutions are assigned a scalarization value of 1.

WEIGHTED_CHEBYSHEV
^^^^^^^^^^^^^^^^^^

.. java:field:: public static final ScalarizationWrapper.ScalarizationType WEIGHTED_CHEBYSHEV
   :outertype: ScalarizationWrapper.ScalarizationType

   Chebyhsev function with weights.

WEIGHTED_PRODUCT
^^^^^^^^^^^^^^^^

.. java:field:: public static final ScalarizationWrapper.ScalarizationType WEIGHTED_PRODUCT
   :outertype: ScalarizationWrapper.ScalarizationType

   Objectives are exponentiated by weights before being multiplied.

WEIGHTED_SUM
^^^^^^^^^^^^

.. java:field:: public static final ScalarizationWrapper.ScalarizationType WEIGHTED_SUM
   :outertype: ScalarizationWrapper.ScalarizationType

   Weighted sum.

