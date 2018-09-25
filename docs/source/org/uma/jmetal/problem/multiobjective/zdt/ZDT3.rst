.. java:import:: org.uma.jmetal.problem.impl AbstractDoubleProblem

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: java.util ArrayList

.. java:import:: java.util List

ZDT3
====

.. java:package:: org.uma.jmetal.problem.multiobjective.zdt
   :noindex:

.. java:type:: @SuppressWarnings public class ZDT3 extends AbstractDoubleProblem

   Class representing problem ZDT3

Constructors
------------
ZDT3
^^^^

.. java:constructor:: public ZDT3()
   :outertype: ZDT3

   Constructor. Creates default instance of problem ZDT3 (30 decision variables)

ZDT3
^^^^

.. java:constructor:: public ZDT3(Integer numberOfVariables)
   :outertype: ZDT3

   Constructor. Creates a instance of ZDT3 problem.

   :param numberOfVariables: Number of variables.

Methods
-------
evalH
^^^^^

.. java:method:: public double evalH(double f, double g)
   :outertype: ZDT3

   Returns the value of the ZDT3 function H.

   :param f: First argument of the function H.
   :param g: Second argument of the function H.

evaluate
^^^^^^^^

.. java:method:: public void evaluate(DoubleSolution solution)
   :outertype: ZDT3

   Evaluate() method

