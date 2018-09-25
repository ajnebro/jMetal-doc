.. java:import:: org.uma.jmetal.problem.impl AbstractDoubleProblem

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: java.util ArrayList

.. java:import:: java.util List

MaF08
=====

.. java:package:: org.uma.jmetal.problem.multiobjective.maf
   :noindex:

.. java:type:: public class MaF08 extends AbstractDoubleProblem

   Class representing problem MaF08

Fields
------
const8
^^^^^^

.. java:field:: public static double const8
   :outertype: MaF08

Constructors
------------
MaF08
^^^^^

.. java:constructor:: public MaF08()
   :outertype: MaF08

   Default constructor

MaF08
^^^^^

.. java:constructor:: public MaF08(Integer numberOfVariables, Integer numberOfObjectives)
   :outertype: MaF08

   Creates a MaF03 problem instance

   :param numberOfVariables: Number of variables
   :param numberOfObjectives: Number of objective functions

Methods
-------
evaluate
^^^^^^^^

.. java:method:: @Override public void evaluate(DoubleSolution solution)
   :outertype: MaF08

   Evaluates a solution

   :param solution: The solution to evaluate

nextPoint
^^^^^^^^^

.. java:method:: public static double[] nextPoint(double arc, double[] startp, double r)
   :outertype: MaF08

polygonpoints
^^^^^^^^^^^^^

.. java:method:: public static double[][] polygonpoints(int m, double r)
   :outertype: MaF08

