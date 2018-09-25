.. java:import:: org.uma.jmetal.problem.impl AbstractDoubleProblem

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: java.util ArrayList

.. java:import:: java.util List

ZDT2
====

.. java:package:: org.uma.jmetal.problem.multiobjective.zdt
   :noindex:

.. java:type:: @SuppressWarnings public class ZDT2 extends AbstractDoubleProblem

   Class representing problem ZDT2

Constructors
------------
ZDT2
^^^^

.. java:constructor:: public ZDT2()
   :outertype: ZDT2

   Constructor. Creates default instance of problem ZDT2 (30 decision variables)

ZDT2
^^^^

.. java:constructor:: public ZDT2(Integer numberOfVariables)
   :outertype: ZDT2

   Constructor. Creates a new ZDT2 problem instance.

   :param numberOfVariables: Number of variables

Methods
-------
evalH
^^^^^

.. java:method:: public double evalH(double f, double g)
   :outertype: ZDT2

   Returns the value of the ZDT2 function H.

   :param f: First argument of the function H.
   :param g: Second argument of the function H.

evaluate
^^^^^^^^

.. java:method:: public void evaluate(DoubleSolution solution)
   :outertype: ZDT2

   Evaluate() method

