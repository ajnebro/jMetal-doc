.. java:import:: org.uma.jmetal.problem.impl AbstractBinaryProblem

.. java:import:: org.uma.jmetal.solution BinarySolution

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: java.util BitSet

ZDT5
====

.. java:package:: org.uma.jmetal.problem.multiobjective.zdt
   :noindex:

.. java:type:: @SuppressWarnings public class ZDT5 extends AbstractBinaryProblem

   Class representing problem ZDT5

Constructors
------------
ZDT5
^^^^

.. java:constructor:: public ZDT5()
   :outertype: ZDT5

   Creates a default instance of problem ZDT5 (11 decision variables)

ZDT5
^^^^

.. java:constructor:: public ZDT5(Integer numberOfVariables)
   :outertype: ZDT5

   Creates a instance of problem ZDT5

   :param numberOfVariables: Number of variables.

Methods
-------
evalG
^^^^^

.. java:method:: public double evalG(BinarySolution solution)
   :outertype: ZDT5

   Returns the value of the ZDT5 function G.

   :param solution: The solution.

evalH
^^^^^

.. java:method:: public double evalH(double f, double g)
   :outertype: ZDT5

   Returns the value of the ZDT5 function H.

   :param f: First argument of the function H.
   :param g: Second argument of the function H.

evalV
^^^^^

.. java:method:: public double evalV(double value)
   :outertype: ZDT5

   Returns the value of the ZDT5 function V.

   :param value: The parameter of V function.

evaluate
^^^^^^^^

.. java:method:: public void evaluate(BinarySolution solution)
   :outertype: ZDT5

   Evaluate() method

getBitsPerVariable
^^^^^^^^^^^^^^^^^^

.. java:method:: @Override protected int getBitsPerVariable(int index)
   :outertype: ZDT5

