.. java:import:: org.uma.jmetal.problem.impl AbstractDoubleProblem

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: java.util ArrayList

.. java:import:: java.util List

MaF06
=====

.. java:package:: org.uma.jmetal.problem.multiobjective.maf
   :noindex:

.. java:type:: public class MaF06 extends AbstractDoubleProblem

   Class representing problem MaF06

Constructors
------------
MaF06
^^^^^

.. java:constructor:: public MaF06()
   :outertype: MaF06

   Default constructor

MaF06
^^^^^

.. java:constructor:: public MaF06(Integer numberOfVariables, Integer numberOfObjectives)
   :outertype: MaF06

   Creates a MaF06 problem instance

   :param numberOfVariables: Number of variables
   :param numberOfObjectives: Number of objective functions

Methods
-------
evaluate
^^^^^^^^

.. java:method:: @Override public void evaluate(DoubleSolution solution)
   :outertype: MaF06

   Evaluates a solution

   :param solution: The solution to evaluate

