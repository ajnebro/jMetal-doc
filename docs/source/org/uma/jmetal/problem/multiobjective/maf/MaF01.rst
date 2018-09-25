.. java:import:: org.uma.jmetal.problem.impl AbstractDoubleProblem

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: java.util ArrayList

.. java:import:: java.util List

MaF01
=====

.. java:package:: org.uma.jmetal.problem.multiobjective.maf
   :noindex:

.. java:type:: public class MaF01 extends AbstractDoubleProblem

   Class representing problem MaF01

Constructors
------------
MaF01
^^^^^

.. java:constructor:: public MaF01()
   :outertype: MaF01

   Default constructor

MaF01
^^^^^

.. java:constructor:: public MaF01(Integer numberOfVariables, Integer numberOfObjectives)
   :outertype: MaF01

   Creates a MaF01 problem instance

   :param numberOfVariables: Number of variables
   :param numberOfObjectives: Number of objective functions

Methods
-------
evaluate
^^^^^^^^

.. java:method:: @Override public void evaluate(DoubleSolution solution)
   :outertype: MaF01

   Evaluates a solution

   :param solution: The solution to evaluate

