.. java:import:: org.uma.jmetal.problem.impl AbstractDoubleProblem

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.util.pseudorandom JMetalRandom

.. java:import:: java.awt.geom Point2D

.. java:import:: java.util ArrayList

.. java:import:: java.util List

MaF09
=====

.. java:package:: org.uma.jmetal.problem.multiobjective.maf
   :noindex:

.. java:type:: public class MaF09 extends AbstractDoubleProblem

   Class representing problem MaF05

Fields
------
M9
^^

.. java:field:: public static int M9
   :outertype: MaF09

maxinter9
^^^^^^^^^

.. java:field:: public static int maxinter9
   :outertype: MaF09

pindex9
^^^^^^^

.. java:field:: public static int pindex9
   :outertype: MaF09

points9
^^^^^^^

.. java:field:: public static double points9
   :outertype: MaF09

Constructors
------------
MaF09
^^^^^

.. java:constructor:: public MaF09()
   :outertype: MaF09

   Default constructor

MaF09
^^^^^

.. java:constructor:: public MaF09(Integer numberOfVariables, Integer numberOfObjectives)
   :outertype: MaF09

   Creates a MaF09 problem instance

   :param numberOfVariables: Number of variables
   :param numberOfObjectives: Number of objective functions

Methods
-------
checkWithJdkGeneralPath
^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public static boolean checkWithJdkGeneralPath(Point2D.Double point, List<Point2D.Double> polygon)
   :outertype: MaF09

evaluate
^^^^^^^^

.. java:method:: @Override public void evaluate(DoubleSolution solution)
   :outertype: MaF09

   Evaluates a solution

   :param solution: The solution to evaluate

generV
^^^^^^

.. java:method:: public static double generV(double lb, double ub)
   :outertype: MaF09

if_infeasible
^^^^^^^^^^^^^

.. java:method:: public static boolean if_infeasible(double[] x)
   :outertype: MaF09

if_inside_polygon
^^^^^^^^^^^^^^^^^

.. java:method:: public static boolean if_inside_polygon(double[] p1, double[][] points)
   :outertype: MaF09

intersection
^^^^^^^^^^^^

.. java:method:: public static double[] intersection(double[] kb1, double[] kb2)
   :outertype: MaF09

line_of_twoP
^^^^^^^^^^^^

.. java:method:: public static double[] line_of_twoP(double[] p1, double[] p2)
   :outertype: MaF09

lines_of_polygon
^^^^^^^^^^^^^^^^

.. java:method:: public double[][] lines_of_polygon(double[][] p)
   :outertype: MaF09

polygonpoints
^^^^^^^^^^^^^

.. java:method:: public static double[][] polygonpoints(int m, double r)
   :outertype: MaF09

