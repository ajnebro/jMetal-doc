.. java:import:: org.uma.jmetal.problem.impl AbstractDoubleProblem

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: java.util ArrayList

.. java:import:: java.util List

ZDT6
====

.. java:package:: org.uma.jmetal.problem.multiobjective.zdt
   :noindex:

.. java:type:: @SuppressWarnings public class ZDT6 extends AbstractDoubleProblem

   Class representing problem ZDT6

Constructors
------------
ZDT6
^^^^

.. java:constructor:: public ZDT6()
   :outertype: ZDT6

   Constructor. Creates a default instance of problem ZDT6 (10 decision variables)

ZDT6
^^^^

.. java:constructor:: public ZDT6(Integer numberOfVariables)
   :outertype: ZDT6

   Creates a instance of problem ZDT6

   :param numberOfVariables: Number of variables

Methods
-------
evalG
^^^^^

.. java:method:: public double evalG(DoubleSolution solution)
   :outertype: ZDT6

   Returns the value of the ZDT6 function G.

   :param solution: Solution

evalH
^^^^^

.. java:method:: public double evalH(double f, double g)
   :outertype: ZDT6

   Returns the value of the ZDT6 function H.

   :param f: First argument of the function H.
   :param g: Second argument of the function H.

evaluate
^^^^^^^^

.. java:method:: public void evaluate(DoubleSolution solution)
   :outertype: ZDT6

   Evaluate() method

