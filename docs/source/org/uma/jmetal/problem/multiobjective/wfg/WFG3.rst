.. java:import:: org.uma.jmetal.solution DoubleSolution

WFG3
====

.. java:package:: org.uma.jmetal.problem.multiobjective.wfg
   :noindex:

.. java:type:: @SuppressWarnings public class WFG3 extends WFG

   This class implements the WFG3 problem Reference: Simon Huband, Luigi Barone, Lyndon While, Phil Hingston A Scalable Multi-objective Test Problem Toolkit. Evolutionary Multi-Criterion Optimization: Third International Conference, EMO 2005. Proceedings, volume 3410 of Lecture Notes in Computer Science

Constructors
------------
WFG3
^^^^

.. java:constructor:: public WFG3()
   :outertype: WFG3

   Creates a default WFG3 instances with 2 position-related parameters 4 distance-related parameters and 2 objectives

WFG3
^^^^

.. java:constructor:: public WFG3(Integer k, Integer l, Integer m)
   :outertype: WFG3

   Creates a WFG3 problem instance

   :param k: Number of position parameters
   :param l: Number of distance parameters
   :param m: Number of objective functions

Methods
-------
evaluate
^^^^^^^^

.. java:method:: public float[] evaluate(float[] z)
   :outertype: WFG3

evaluate
^^^^^^^^

.. java:method:: public void evaluate(DoubleSolution solution)
   :outertype: WFG3

   Evaluates a solution

   :param solution: The solution to runAlgorithm
   :throws org.uma.jmetal.util.JMetalException:

t1
^^

.. java:method:: public float[] t1(float[] z, int k)
   :outertype: WFG3

   WFG3 t1 transformation

t2
^^

.. java:method:: public float[] t2(float[] z, int k)
   :outertype: WFG3

   WFG3 t2 transformation

t3
^^

.. java:method:: public float[] t3(float[] z, int k, int M)
   :outertype: WFG3

   WFG3 t3 transformation

