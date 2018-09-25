.. java:import:: org.uma.jmetal.problem.impl AbstractDoubleProblem

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: java.util ArrayList

.. java:import:: java.util List

ZDT1
====

.. java:package:: org.uma.jmetal.problem.multiobjective.zdt
   :noindex:

.. java:type:: @SuppressWarnings public class ZDT1 extends AbstractDoubleProblem

   Class representing problem ZDT1

Constructors
------------
ZDT1
^^^^

.. java:constructor:: public ZDT1()
   :outertype: ZDT1

   Constructor. Creates default instance of problem ZDT1 (30 decision variables)

ZDT1
^^^^

.. java:constructor:: public ZDT1(Integer numberOfVariables)
   :outertype: ZDT1

   Creates a new instance of problem ZDT1.

   :param numberOfVariables: Number of variables.

Methods
-------
evalH
^^^^^

.. java:method:: public double evalH(double f, double g)
   :outertype: ZDT1

   Returns the value of the ZDT1 function H.

   :param f: First argument of the function H.
   :param g: Second argument of the function H.

evaluate
^^^^^^^^

.. java:method:: public void evaluate(DoubleSolution solution)
   :outertype: ZDT1

   Evaluate() method

