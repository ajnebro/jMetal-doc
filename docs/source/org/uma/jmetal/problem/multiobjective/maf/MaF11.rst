.. java:import:: org.uma.jmetal.problem.impl AbstractDoubleProblem

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: java.util ArrayList

.. java:import:: java.util List

MaF11
=====

.. java:package:: org.uma.jmetal.problem.multiobjective.maf
   :noindex:

.. java:type:: public class MaF11 extends AbstractDoubleProblem

   Class representing problem MaF11

Fields
------
K11
^^^

.. java:field:: public static int K11
   :outertype: MaF11

Constructors
------------
MaF11
^^^^^

.. java:constructor:: public MaF11()
   :outertype: MaF11

   Default constructor

MaF11
^^^^^

.. java:constructor:: public MaF11(Integer numberOfVariables, Integer numberOfObjectives)
   :outertype: MaF11

   Creates a MaF11 problem instance

   :param numberOfVariables: Number of variables
   :param numberOfObjectives: Number of objective functions

Methods
-------
evaluate
^^^^^^^^

.. java:method:: @Override public void evaluate(DoubleSolution solution)
   :outertype: MaF11

   Evaluates a solution

   :param solution: The solution to evaluate

