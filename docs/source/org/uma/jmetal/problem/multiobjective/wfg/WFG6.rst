.. java:import:: org.uma.jmetal.solution DoubleSolution

WFG6
====

.. java:package:: org.uma.jmetal.problem.multiobjective.wfg
   :noindex:

.. java:type:: @SuppressWarnings public class WFG6 extends WFG

   This class implements the WFG6 problem Reference: Simon Huband, Luigi Barone, Lyndon While, Phil Hingston A Scalable Multi-objective Test Problem Toolkit. Evolutionary Multi-Criterion Optimization: Third International Conference, EMO 2005. Proceedings, volume 3410 of Lecture Notes in Computer Science

Constructors
------------
WFG6
^^^^

.. java:constructor:: public WFG6()
   :outertype: WFG6

   Creates a default WFG6 with 2 position-related parameters, 4 distance-related parameters, and 2 objectives

WFG6
^^^^

.. java:constructor:: public WFG6(Integer k, Integer l, Integer m)
   :outertype: WFG6

   Creates a WFG6 problem instance

   :param k: Number of position parameters
   :param l: Number of distance parameters
   :param m: Number of objective functions

Methods
-------
evaluate
^^^^^^^^

.. java:method:: public float[] evaluate(float[] z)
   :outertype: WFG6

   Evaluate() method

evaluate
^^^^^^^^

.. java:method:: public void evaluate(DoubleSolution solution)
   :outertype: WFG6

   Evaluates a solution

   :param solution: The solution to runAlgorithm
   :throws org.uma.jmetal.util.JMetalException:

t1
^^

.. java:method:: public float[] t1(float[] z, int k)
   :outertype: WFG6

   WFG6 t1 transformation

t2
^^

.. java:method:: public float[] t2(float[] z, int k, int M)
   :outertype: WFG6

   WFG6 t2 transformation

