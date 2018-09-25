.. java:import:: org.uma.jmetal.problem.impl AbstractDoubleProblem

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: java.util ArrayList

.. java:import:: java.util List

ZDT4
====

.. java:package:: org.uma.jmetal.problem.multiobjective.zdt
   :noindex:

.. java:type:: @SuppressWarnings public class ZDT4 extends AbstractDoubleProblem

   Class representing problem ZDT4

Constructors
------------
ZDT4
^^^^

.. java:constructor:: public ZDT4()
   :outertype: ZDT4

   Constructor. Creates a default instance of problem ZDT4 (10 decision variables

ZDT4
^^^^

.. java:constructor:: public ZDT4(Integer numberOfVariables)
   :outertype: ZDT4

   Creates a instance of problem ZDT4.

   :param numberOfVariables: Number of variables.

Methods
-------
evalG
^^^^^

.. java:method:: public double evalG(DoubleSolution solution)
   :outertype: ZDT4

   Returns the value of the ZDT4 function G.

   :param solution: Solution

evalH
^^^^^

.. java:method:: public double evalH(double f, double g)
   :outertype: ZDT4

   Returns the value of the ZDT4 function H.

   :param f: First argument of the function H.
   :param g: Second argument of the function H.

evaluate
^^^^^^^^

.. java:method:: public void evaluate(DoubleSolution solution)
   :outertype: ZDT4

   Evaluate() method

