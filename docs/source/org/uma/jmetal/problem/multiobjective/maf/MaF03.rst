.. java:import:: org.uma.jmetal.problem.impl AbstractDoubleProblem

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: java.util ArrayList

.. java:import:: java.util List

MaF03
=====

.. java:package:: org.uma.jmetal.problem.multiobjective.maf
   :noindex:

.. java:type:: public class MaF03 extends AbstractDoubleProblem

   Class representing problem MaF03, convex DTLZ3

Constructors
------------
MaF03
^^^^^

.. java:constructor:: public MaF03()
   :outertype: MaF03

   Default constructor

MaF03
^^^^^

.. java:constructor:: public MaF03(Integer numberOfVariables, Integer numberOfObjectives)
   :outertype: MaF03

   Creates a MaF03 problem instance

   :param numberOfVariables: Number of variables
   :param numberOfObjectives: Number of objective functions

Methods
-------
evaluate
^^^^^^^^

.. java:method:: @Override public void evaluate(DoubleSolution solution)
   :outertype: MaF03

   Evaluates a solution

   :param solution: The solution to evaluate

