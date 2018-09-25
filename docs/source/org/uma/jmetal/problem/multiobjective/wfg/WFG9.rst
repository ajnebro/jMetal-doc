.. java:import:: org.uma.jmetal.solution DoubleSolution

WFG9
====

.. java:package:: org.uma.jmetal.problem.multiobjective.wfg
   :noindex:

.. java:type:: @SuppressWarnings public class WFG9 extends WFG

   Creates a default WFG9 problem with 2 position-related parameters, 4 distance-related parameters, and 2 objectives

Constructors
------------
WFG9
^^^^

.. java:constructor:: public WFG9()
   :outertype: WFG9

   Creates a default WFG9 with 2 position-related parameters, 4 distance-related parameters, and 2 objectives

WFG9
^^^^

.. java:constructor:: public WFG9(Integer k, Integer l, Integer m)
   :outertype: WFG9

   Creates a WFG9 problem instance

   :param k: Number of position variables
   :param l: Number of distance variables
   :param m: Number of objective functions

Methods
-------
evaluate
^^^^^^^^

.. java:method:: public float[] evaluate(float[] z)
   :outertype: WFG9

   Evaluate() method

evaluate
^^^^^^^^

.. java:method:: public void evaluate(DoubleSolution solution)
   :outertype: WFG9

   Evaluates a solution

   :param solution: The solution to runAlgorithm
   :throws org.uma.jmetal.util.JMetalException:

t1
^^

.. java:method:: public float[] t1(float[] z, int k)
   :outertype: WFG9

   WFG9 t1 transformation

t2
^^

.. java:method:: public float[] t2(float[] z, int k)
   :outertype: WFG9

   WFG9 t2 transformation

t3
^^

.. java:method:: public float[] t3(float[] z, int k, int M)
   :outertype: WFG9

   WFG9 t3 transformation

