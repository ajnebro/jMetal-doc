.. java:import:: org.uma.jmetal.problem.impl AbstractDoubleProblem

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: java.util ArrayList

.. java:import:: java.util List

MaF12
=====

.. java:package:: org.uma.jmetal.problem.multiobjective.maf
   :noindex:

.. java:type:: public class MaF12 extends AbstractDoubleProblem

   Class representing problem MaF12

Fields
------
K12
^^^

.. java:field:: public static int K12
   :outertype: MaF12

Constructors
------------
MaF12
^^^^^

.. java:constructor:: public MaF12()
   :outertype: MaF12

   Default constructor

MaF12
^^^^^

.. java:constructor:: public MaF12(Integer numberOfVariables, Integer numberOfObjectives)
   :outertype: MaF12

   Creates a MaF12 problem instance

   :param numberOfVariables: Number of variables
   :param numberOfObjectives: Number of objective functions

Methods
-------
evaluate
^^^^^^^^

.. java:method:: @Override public void evaluate(DoubleSolution solution)
   :outertype: MaF12

   Evaluates a solution

   :param solution: The solution to evaluate

