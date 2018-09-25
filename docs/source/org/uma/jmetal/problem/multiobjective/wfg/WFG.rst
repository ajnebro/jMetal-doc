.. java:import:: org.uma.jmetal.problem.impl AbstractDoubleProblem

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.solution.impl DefaultDoubleSolution

.. java:import:: java.util ArrayList

.. java:import:: java.util List

.. java:import:: java.util Random

WFG
===

.. java:package:: org.uma.jmetal.problem.multiobjective.wfg
   :noindex:

.. java:type:: @SuppressWarnings public abstract class WFG extends AbstractDoubleProblem

   Implements a reference abstract class for all wfg org.uma.test problem Reference: Simon Huband, Luigi Barone, Lyndon While, Phil Hingston A Scalable Multi-objective Test Problem Toolkit. Evolutionary Multi-Criterion Optimization: Third International Conference, EMO 2005. Proceedings, volume 3410 of Lecture Notes in Computer Science

Fields
------
a
^

.. java:field:: protected int[] a
   :outertype: WFG

d
^

.. java:field:: protected int d
   :outertype: WFG

k
^

.. java:field:: protected int k
   :outertype: WFG

l
^

.. java:field:: protected int l
   :outertype: WFG

m
^

.. java:field:: protected int m
   :outertype: WFG

random
^^^^^^

.. java:field:: protected Random random
   :outertype: WFG

s
^

.. java:field:: protected int[] s
   :outertype: WFG

Constructors
------------
WFG
^^^

.. java:constructor:: public WFG(Integer k, Integer l, Integer M)
   :outertype: WFG

   Constructor Creates a wfg problem

   :param k: position-related parameters
   :param l: distance-related parameters
   :param M: Number of objectives

Methods
-------
calculateX
^^^^^^^^^^

.. java:method:: public float[] calculateX(float[] t)
   :outertype: WFG

   Gets the x vector

correctTo01
^^^^^^^^^^^

.. java:method:: public float correctTo01(float a)
   :outertype: WFG

createSolution
^^^^^^^^^^^^^^

.. java:method:: @Override public DoubleSolution createSolution()
   :outertype: WFG

evaluate
^^^^^^^^

.. java:method:: public abstract float[] evaluate(float[] variables)
   :outertype: WFG

   Evaluates a solution

   :param variables: The solution to evaluate
   :return: a double [] with the evaluation results

normalise
^^^^^^^^^

.. java:method:: public float[] normalise(float[] z)
   :outertype: WFG

   Normalizes a vector (consulte wfg toolkit reference)

subVector
^^^^^^^^^

.. java:method:: public float[] subVector(float[] z, int head, int tail)
   :outertype: WFG

   Gets a subvector of a given vector (Head inclusive and tail inclusive)

   :param z: the vector
   :return: the subvector

