.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: org.uma.jmetal.util JMetalLogger

.. java:import:: java.util.logging Level

WFG1
====

.. java:package:: org.uma.jmetal.problem.multiobjective.wfg
   :noindex:

.. java:type:: @SuppressWarnings public class WFG1 extends WFG

   This class implements the WFG1 problem Reference: Simon Huband, Luigi Barone, Lyndon While, Phil Hingston A Scalable Multi-objective Test Problem Toolkit. Evolutionary Multi-Criterion Optimization: Third International Conference, EMO 2005. Proceedings, volume 3410 of Lecture Notes in Computer Science

Constructors
------------
WFG1
^^^^

.. java:constructor:: public WFG1()
   :outertype: WFG1

   Constructor Creates a default WFG1 instance with 2 position-related parameters 4 distance-related parameters and 2 objectives

WFG1
^^^^

.. java:constructor:: public WFG1(Integer k, Integer l, Integer m)
   :outertype: WFG1

   Creates a WFG1 problem instance

   :param k: Number of position parameters
   :param l: Number of distance parameters
   :param m: Number of objective functions

Methods
-------
evaluate
^^^^^^^^

.. java:method:: public float[] evaluate(float[] z)
   :outertype: WFG1

   Evaluate

evaluate
^^^^^^^^

.. java:method:: public void evaluate(DoubleSolution solution)
   :outertype: WFG1

   Evaluates a solution

   :param solution: The solution to runAlgorithm
   :throws org.uma.jmetal.util.JMetalException:

t1
^^

.. java:method:: public float[] t1(float[] z, int k)
   :outertype: WFG1

   WFG1 t1 transformation

t2
^^

.. java:method:: public float[] t2(float[] z, int k)
   :outertype: WFG1

   WFG1 t2 transformation

t3
^^

.. java:method:: public float[] t3(float[] z) throws JMetalException
   :outertype: WFG1

   WFG1 t3 transformation

   :throws org.uma.jmetal.util.JMetalException:

t4
^^

.. java:method:: public float[] t4(float[] z, int k, int M)
   :outertype: WFG1

   WFG1 t4 transformation

