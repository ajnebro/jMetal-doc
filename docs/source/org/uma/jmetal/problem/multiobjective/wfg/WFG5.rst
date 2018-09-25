.. java:import:: org.uma.jmetal.solution DoubleSolution

WFG5
====

.. java:package:: org.uma.jmetal.problem.multiobjective.wfg
   :noindex:

.. java:type:: @SuppressWarnings public class WFG5 extends WFG

   This class implements the WFG5 problem Reference: Simon Huband, Luigi Barone, Lyndon While, Phil Hingston A Scalable Multi-objective Test Problem Toolkit. Evolutionary Multi-Criterion Optimization: Third International Conference, EMO 2005. Proceedings, volume 3410 of Lecture Notes in Computer Science

Constructors
------------
WFG5
^^^^

.. java:constructor:: public WFG5()
   :outertype: WFG5

   Creates a default WFG5 instance with 2 position-related parameters 4 distance-related parameters and 2 objectives

WFG5
^^^^

.. java:constructor:: public WFG5(Integer k, Integer l, Integer m)
   :outertype: WFG5

   Creates a WFG5 problem instance

   :param k: Number of position parameters
   :param l: Number of distance parameters
   :param m: Number of objective functions

Methods
-------
evaluate
^^^^^^^^

.. java:method:: public float[] evaluate(float[] z)
   :outertype: WFG5

   Evaluate() method

evaluate
^^^^^^^^

.. java:method:: public void evaluate(DoubleSolution solution)
   :outertype: WFG5

   Evaluates a solution

   :param solution: The solution to runAlgorithm
   :throws org.uma.jmetal.util.JMetalException:

t1
^^

.. java:method:: public float[] t1(float[] z, int k)
   :outertype: WFG5

   WFG5 t1 transformation

t2
^^

.. java:method:: public float[] t2(float[] z, int k, int M)
   :outertype: WFG5

   WFG5 t2 transformation

