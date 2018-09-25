.. java:import:: org.uma.jmetal.problem.impl AbstractDoubleProblem

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: java.util ArrayList

.. java:import:: java.util List

MaF07
=====

.. java:package:: org.uma.jmetal.problem.multiobjective.maf
   :noindex:

.. java:type:: public class MaF07 extends AbstractDoubleProblem

   Class representing problem MaF07

Constructors
------------
MaF07
^^^^^

.. java:constructor:: public MaF07()
   :outertype: MaF07

   Default constructor

MaF07
^^^^^

.. java:constructor:: public MaF07(Integer numberOfVariables, Integer numberOfObjectives)
   :outertype: MaF07

   Creates a MaF07 problem instance

   :param numberOfVariables: Number of variables
   :param numberOfObjectives: Number of objective functions

Methods
-------
evaluate
^^^^^^^^

.. java:method:: @Override public void evaluate(DoubleSolution solution)
   :outertype: MaF07

   Evaluates a solution

   :param solution: The solution to evaluate

