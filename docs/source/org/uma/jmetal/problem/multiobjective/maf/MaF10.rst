.. java:import:: org.uma.jmetal.problem.impl AbstractDoubleProblem

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: java.util ArrayList

.. java:import:: java.util List

MaF10
=====

.. java:package:: org.uma.jmetal.problem.multiobjective.maf
   :noindex:

.. java:type:: public class MaF10 extends AbstractDoubleProblem

   Class representing problem MaF10

Fields
------
K10
^^^

.. java:field:: public static int K10
   :outertype: MaF10

Constructors
------------
MaF10
^^^^^

.. java:constructor:: public MaF10()
   :outertype: MaF10

   Default constructor

MaF10
^^^^^

.. java:constructor:: public MaF10(Integer numberOfVariables, Integer numberOfObjectives)
   :outertype: MaF10

   Creates a MaF10 problem instance

   :param numberOfVariables: Number of variables
   :param numberOfObjectives: Number of objective functions

Methods
-------
evaluate
^^^^^^^^

.. java:method:: @Override public void evaluate(DoubleSolution solution)
   :outertype: MaF10

   Evaluates a solution

   :param solution: The solution to evaluate

