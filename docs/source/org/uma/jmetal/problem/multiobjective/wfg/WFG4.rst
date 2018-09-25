.. java:import:: org.uma.jmetal.solution DoubleSolution

WFG4
====

.. java:package:: org.uma.jmetal.problem.multiobjective.wfg
   :noindex:

.. java:type:: @SuppressWarnings public class WFG4 extends WFG

   This class implements the WFG4 problem Reference: Simon Huband, Luigi Barone, Lyndon While, Phil Hingston A Scalable Multi-objective Test Problem Toolkit. Evolutionary Multi-Criterion Optimization: Third International Conference, EMO 2005. Proceedings, volume 3410 of Lecture Notes in Computer Science

Constructors
------------
WFG4
^^^^

.. java:constructor:: public WFG4()
   :outertype: WFG4

   Creates a default WFG4 with 2 position-related parameter, 4 distance-related parameter and 2 objectives

WFG4
^^^^

.. java:constructor:: public WFG4(Integer k, Integer l, Integer m)
   :outertype: WFG4

   Creates a WFG4 problem instance

   :param k: Number of position parameters
   :param l: Number of distance parameters
   :param m: Number of objective functions

Methods
-------
evaluate
^^^^^^^^

.. java:method:: public float[] evaluate(float[] z)
   :outertype: WFG4

   Evaluate() method

evaluate
^^^^^^^^

.. java:method:: public void evaluate(DoubleSolution solution)
   :outertype: WFG4

   Evaluates a solution

   :param solution: The solution to runAlgorithm
   :throws org.uma.jmetal.util.JMetalException:

t1
^^

.. java:method:: public float[] t1(float[] z, int k)
   :outertype: WFG4

   WFG4 t1 transformation

t2
^^

.. java:method:: public float[] t2(float[] z, int k, int M)
   :outertype: WFG4

   WFG4 t2 transformation

