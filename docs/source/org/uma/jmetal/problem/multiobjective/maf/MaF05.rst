.. java:import:: org.uma.jmetal.problem.impl AbstractDoubleProblem

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: java.util ArrayList

.. java:import:: java.util List

MaF05
=====

.. java:package:: org.uma.jmetal.problem.multiobjective.maf
   :noindex:

.. java:type:: public class MaF05 extends AbstractDoubleProblem

   Class representing problem MaF05

Fields
------
const5
^^^^^^

.. java:field:: public static double const5
   :outertype: MaF05

Constructors
------------
MaF05
^^^^^

.. java:constructor:: public MaF05()
   :outertype: MaF05

   Default constructor

MaF05
^^^^^

.. java:constructor:: public MaF05(Integer numberOfVariables, Integer numberOfObjectives)
   :outertype: MaF05

   Creates a MaF05 problem instance

   :param numberOfVariables: Number of variables
   :param numberOfObjectives: Number of objective functions

Methods
-------
evaluate
^^^^^^^^

.. java:method:: @Override public void evaluate(DoubleSolution solution)
   :outertype: MaF05

   Evaluates a solution

   :param solution: The solution to evaluate

