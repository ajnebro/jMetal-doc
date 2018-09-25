.. java:import:: org.uma.jmetal.problem.impl AbstractDoubleProblem

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: java.util ArrayList

.. java:import:: java.util List

MaF15
=====

.. java:package:: org.uma.jmetal.problem.multiobjective.maf
   :noindex:

.. java:type:: public class MaF15 extends AbstractDoubleProblem

   Class representing problem MaF15

Fields
------
nk15
^^^^

.. java:field:: public static int nk15
   :outertype: MaF15

sublen15
^^^^^^^^

.. java:field:: public static int sublen15
   :outertype: MaF15

Constructors
------------
MaF15
^^^^^

.. java:constructor:: public MaF15()
   :outertype: MaF15

   Default constructor

MaF15
^^^^^

.. java:constructor:: public MaF15(Integer numberOfVariables, Integer numberOfObjectives)
   :outertype: MaF15

   Creates a MaF15 problem instance

   :param numberOfVariables: Number of variables
   :param numberOfObjectives: Number of objective functions

Methods
-------
Griewank
^^^^^^^^

.. java:method:: public static double Griewank(double[] x)
   :outertype: MaF15

Sphere
^^^^^^

.. java:method:: public static double Sphere(double[] x)
   :outertype: MaF15

evaluate
^^^^^^^^

.. java:method:: @Override public void evaluate(DoubleSolution solution)
   :outertype: MaF15

   Evaluates a solution

   :param solution: The solution to evaluate

