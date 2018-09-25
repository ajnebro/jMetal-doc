.. java:import:: org.uma.jmetal.problem.impl AbstractDoubleProblem

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: java.util ArrayList

.. java:import:: java.util List

MaF13
=====

.. java:package:: org.uma.jmetal.problem.multiobjective.maf
   :noindex:

.. java:type:: public class MaF13 extends AbstractDoubleProblem

   Class representing problem MaF13

Constructors
------------
MaF13
^^^^^

.. java:constructor:: public MaF13()
   :outertype: MaF13

   Default constructor

MaF13
^^^^^

.. java:constructor:: public MaF13(Integer numberOfVariables, Integer numberOfObjectives)
   :outertype: MaF13

   Creates a MaF13 problem instance

   :param numberOfVariables: Number of variables
   :param numberOfObjectives: Number of objective functions

Methods
-------
evaluate
^^^^^^^^

.. java:method:: @Override public void evaluate(DoubleSolution solution)
   :outertype: MaF13

   Evaluates a solution

   :param solution: The solution to evaluate

