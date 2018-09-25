.. java:import:: org.uma.jmetal.problem.impl AbstractDoubleProblem

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: java.util ArrayList

.. java:import:: java.util List

MaF02
=====

.. java:package:: org.uma.jmetal.problem.multiobjective.maf
   :noindex:

.. java:type:: public class MaF02 extends AbstractDoubleProblem

   Class representing problem MaF02, DTLZ2BZ

Fields
------
const2
^^^^^^

.. java:field:: public static int const2
   :outertype: MaF02

Constructors
------------
MaF02
^^^^^

.. java:constructor:: public MaF02()
   :outertype: MaF02

   Default constructor

MaF02
^^^^^

.. java:constructor:: public MaF02(Integer numberOfVariables, Integer numberOfObjectives)
   :outertype: MaF02

   Creates a MaF02 problem instance

   :param numberOfVariables: Number of variables
   :param numberOfObjectives: Number of objective functions

Methods
-------
evaluate
^^^^^^^^

.. java:method:: @Override public void evaluate(DoubleSolution solution)
   :outertype: MaF02

   Evaluates a solution

   :param solution: The solution to evaluate

