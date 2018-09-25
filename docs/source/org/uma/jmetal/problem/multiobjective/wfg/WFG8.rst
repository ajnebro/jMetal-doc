.. java:import:: org.uma.jmetal.solution DoubleSolution

WFG8
====

.. java:package:: org.uma.jmetal.problem.multiobjective.wfg
   :noindex:

.. java:type:: @SuppressWarnings public class WFG8 extends WFG

   Creates a default WFG8 problem with 2 position-related parameters, 4 distance-related parameters, and 2 objectives

Constructors
------------
WFG8
^^^^

.. java:constructor:: public WFG8()
   :outertype: WFG8

   Creates a default WFG8 with 2 position-related parameters, 4 distance-related parameters, and 2 objectives

WFG8
^^^^

.. java:constructor:: public WFG8(Integer k, Integer l, Integer m)
   :outertype: WFG8

   Creates a WFG8 problem instance

   :param k: Number of position parameters
   :param l: Number of distance parameters
   :param m: Number of objective functions

Methods
-------
evaluate
^^^^^^^^

.. java:method:: public float[] evaluate(float[] z)
   :outertype: WFG8

   Evaluate() method

evaluate
^^^^^^^^

.. java:method:: public void evaluate(DoubleSolution solution)
   :outertype: WFG8

   Evaluates a solution

   :param solution: The solution to runAlgorithm
   :throws org.uma.jmetal.util.JMetalException:

t1
^^

.. java:method:: public float[] t1(float[] z, int k)
   :outertype: WFG8

   WFG8 t1 transformation

t2
^^

.. java:method:: public float[] t2(float[] z, int k)
   :outertype: WFG8

   WFG8 t2 transformation

t3
^^

.. java:method:: public float[] t3(float[] z, int k, int M)
   :outertype: WFG8

   WFG8 t3 transformation

