.. java:import:: org.uma.jmetal.solution DoubleSolution

WFG7
====

.. java:package:: org.uma.jmetal.problem.multiobjective.wfg
   :noindex:

.. java:type:: @SuppressWarnings public class WFG7 extends WFG

Constructors
------------
WFG7
^^^^

.. java:constructor:: public WFG7()
   :outertype: WFG7

   Creates a default WFG7 problem with 2 position-related parameters, 4 distance-related parameters, and 2 objectives

WFG7
^^^^

.. java:constructor:: public WFG7(Integer k, Integer l, Integer m)
   :outertype: WFG7

   Creates a WFG7 problem instance

   :param k: Number of position parameters
   :param l: Number of distance parameters
   :param m: Number of objective functions

Methods
-------
evaluate
^^^^^^^^

.. java:method:: public float[] evaluate(float[] z)
   :outertype: WFG7

   Evaluate() method

evaluate
^^^^^^^^

.. java:method:: public void evaluate(DoubleSolution solution)
   :outertype: WFG7

   Evaluate() method

t1
^^

.. java:method:: public float[] t1(float[] z, int k)
   :outertype: WFG7

   WFG7 t1 transformation

t2
^^

.. java:method:: public float[] t2(float[] z, int k)
   :outertype: WFG7

   WFG7 t2 transformation

t3
^^

.. java:method:: public float[] t3(float[] z, int k, int M)
   :outertype: WFG7

   WFG7 t3 transformation

