.. java:import:: org.uma.jmetal.solution DoubleSolution

WFG2
====

.. java:package:: org.uma.jmetal.problem.multiobjective.wfg
   :noindex:

.. java:type:: @SuppressWarnings public class WFG2 extends WFG

   This class implements the WFG2 problem Reference: Simon Huband, Luigi Barone, Lyndon While, Phil Hingston A Scalable Multi-objective Test Problem Toolkit. Evolutionary Multi-Criterion Optimization: Third International Conference, EMO 2005. Proceedings, volume 3410 of Lecture Notes in Computer Science

Constructors
------------
WFG2
^^^^

.. java:constructor:: public WFG2()
   :outertype: WFG2

   Creates a default WFG2 instance with 2 position-related parameters 4 distance-related parameters and 2 objectives

WFG2
^^^^

.. java:constructor:: public WFG2(Integer k, Integer l, Integer m)
   :outertype: WFG2

   Creates a WFG2 problem instance

   :param k: Number of position parameters
   :param l: Number of distance parameters
   :param m: Number of objective functions

Methods
-------
evaluate
^^^^^^^^

.. java:method:: public float[] evaluate(float[] z)
   :outertype: WFG2

evaluate
^^^^^^^^

.. java:method:: public void evaluate(DoubleSolution solution)
   :outertype: WFG2

   Evaluates a solution

   :param solution: The solution to runAlgorithm

t1
^^

.. java:method:: public float[] t1(float[] z, int k)
   :outertype: WFG2

   WFG2 t1 transformation

t2
^^

.. java:method:: public float[] t2(float[] z, int k)
   :outertype: WFG2

   WFG2 t2 transformation

t3
^^

.. java:method:: public float[] t3(float[] z, int k, int M)
   :outertype: WFG2

   WFG2 t3 transformation

