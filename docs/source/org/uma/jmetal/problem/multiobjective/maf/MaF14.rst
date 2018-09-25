.. java:import:: org.uma.jmetal.problem.impl AbstractDoubleProblem

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: java.util ArrayList

.. java:import:: java.util List

MaF14
=====

.. java:package:: org.uma.jmetal.problem.multiobjective.maf
   :noindex:

.. java:type:: public class MaF14 extends AbstractDoubleProblem

   Class representing problem MaF14

Fields
------
nk14
^^^^

.. java:field:: public static int nk14
   :outertype: MaF14

sublen14
^^^^^^^^

.. java:field:: public static int sublen14
   :outertype: MaF14

Constructors
------------
MaF14
^^^^^

.. java:constructor:: public MaF14()
   :outertype: MaF14

   Default constructor

MaF14
^^^^^

.. java:constructor:: public MaF14(Integer numberOfVariables, Integer numberOfObjectives)
   :outertype: MaF14

   Creates a MaF14 problem instance

   :param numberOfVariables: Number of variables
   :param numberOfObjectives: Number of objective functions

Methods
-------
Rastrigin
^^^^^^^^^

.. java:method:: public static double Rastrigin(double[] x)
   :outertype: MaF14

Rosenbrock
^^^^^^^^^^

.. java:method:: public static double Rosenbrock(double[] x)
   :outertype: MaF14

evaluate
^^^^^^^^

.. java:method:: @Override public void evaluate(DoubleSolution solution)
   :outertype: MaF14

