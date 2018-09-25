.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util.extremevalues.impl FrontExtremeValues

.. java:import:: org.uma.jmetal.util.front.imp ArrayFront

.. java:import:: java.util Collections

.. java:import:: java.util List

ScalarizationUtils
==================

.. java:package:: org.uma.jmetal.algorithm.multiobjective.espea.util
   :noindex:

.. java:type:: public class ScalarizationUtils

   A class that contains methods for computing the scalarization values of solutions. A scalarization value is an aggregation of the objective values that maps to the real numbers, e.g. the weighted sum.

   Scalarization values are stored as \ :java:ref:`ScalarizationValue`\  in the solutions.

   :author: Marlon Braun

Methods
-------
angleUtility
^^^^^^^^^^^^

.. java:method:: public static <S extends Solution<?>> void angleUtility(List<S> solutionsList)
   :outertype: ScalarizationUtils

   Scalarization values based on angle utility (see Angle-based Preference Models in Multi-objective Optimization by Braun et al.). Extreme points are computed from the list of solutions.

   :param solutionsList: A list of solutions.

angleUtility
^^^^^^^^^^^^

.. java:method:: public static <S extends Solution<?>> void angleUtility(List<S> solutionsList, double[][] extremePoints)
   :outertype: ScalarizationUtils

   Scalarization values based on angle utility (see Angle-based Preference Models in Multi-objective Optimization by Braun et al.).

   :param solutionsList: A list of solutions.
   :param extremePoints: used for angle computation.

chebyshev
^^^^^^^^^

.. java:method:: public static <S extends Solution<?>> void chebyshev(List<S> solutionsList)
   :outertype: ScalarizationUtils

   Scalarization values based on the Chebyshev function. The ideal point is computed from the list of solutions.

   :param solutionsList: A list of solutions.

chebyshev
^^^^^^^^^

.. java:method:: public static <S extends Solution<?>> void chebyshev(List<S> solutionsList, double[] idealValues)
   :outertype: ScalarizationUtils

   Scalarization values based on the Chebyshev function.

   :param solutionsList: A list of solutions.
   :param idealValues: The ideal point

nash
^^^^

.. java:method:: public static <S extends Solution<?>> void nash(List<S> solutionsList)
   :outertype: ScalarizationUtils

   Scalarization values based on the Nash bargaining solution. The disagreement point is computed based on the list of solutions.

   :param solutionsList: A list of solutions.

nash
^^^^

.. java:method:: public static <S extends Solution<?>> void nash(List<S> solutionsList, double[] nadirValues)
   :outertype: ScalarizationUtils

   Scalarization values based on the Nash bargaining solution.

   :param solutionsList: A list of solutions.
   :param nadirValues: The disagreement point.

productOfObjectives
^^^^^^^^^^^^^^^^^^^

.. java:method:: public static <S extends Solution<?>> void productOfObjectives(List<S> solutionsList)
   :outertype: ScalarizationUtils

   Objective values are multiplied.

   :param solutionsList: A list of solutions.

sumOfObjectives
^^^^^^^^^^^^^^^

.. java:method:: public static <S extends Solution<?>> void sumOfObjectives(List<S> solutionsList)
   :outertype: ScalarizationUtils

   Scalarization values is computed by summing objective values.

   :param solutionsList: A list of solutions.

tradeoffUtility
^^^^^^^^^^^^^^^

.. java:method:: public static <S extends Solution<?>> void tradeoffUtility(List<S> solutionsList)
   :outertype: ScalarizationUtils

   Scalarization values based on tradeoff utility, also known as proper utility (see "Theory and Algorithm for Finding Knees" by Shukla et al.)

   :param solutionsList: A list of solutions.

uniform
^^^^^^^

.. java:method:: public static <S extends Solution<?>> void uniform(List<S> solutionsList)
   :outertype: ScalarizationUtils

   Uniform preferences. Each solution is assigned a scalarization value of 1.0.

   :param solutionsList: A list of solutions.

weightedChebyshev
^^^^^^^^^^^^^^^^^

.. java:method:: public static <S extends Solution<?>> void weightedChebyshev(List<S> solutionsList, double[] weights)
   :outertype: ScalarizationUtils

   Chebyhsev function with weighted objectives.

   :param solutionsList: A list of solutions.
   :param weights: Constants by which ideal values and objective values are multiplied.

weightedChebyshev
^^^^^^^^^^^^^^^^^

.. java:method:: public static <S extends Solution<?>> void weightedChebyshev(List<S> solutionsList, double[] idealValues, double[] weights)
   :outertype: ScalarizationUtils

   Scalarization values based on the weighted Chebyshev function.

   :param solutionsList: A list of solutions.
   :param idealValues: The ideal point.
   :param weights: Constants by which ideal values and objective values are multiplied.

weightedProduct
^^^^^^^^^^^^^^^

.. java:method:: public static <S extends Solution<?>> void weightedProduct(List<S> solutionsList, double[] weights)
   :outertype: ScalarizationUtils

   Objectives are exponentiated by a positive weight and afterwards multiplied.

   :param solutionsList: A list of solutions.
   :param weights: Weights by objectives are exponentiated

weightedSum
^^^^^^^^^^^

.. java:method:: public static <S extends Solution<?>> void weightedSum(List<S> solutionsList, double[] weights)
   :outertype: ScalarizationUtils

   Objective values are multiplied by weights and summed. Weights should always be positive.

   :param solutionsList: A list of solutions.
   :param weights: Positive constants by which objectives are summed.

