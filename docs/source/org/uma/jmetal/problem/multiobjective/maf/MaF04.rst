.. java:import:: org.uma.jmetal.problem.impl AbstractDoubleProblem

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: java.util ArrayList

.. java:import:: java.util List

MaF04
=====

.. java:package:: org.uma.jmetal.problem.multiobjective.maf
   :noindex:

.. java:type:: public class MaF04 extends AbstractDoubleProblem

   Class representing problem MaF04

Fields
------
const4
^^^^^^

.. java:field:: public static double const4
   :outertype: MaF04

Constructors
------------
MaF04
^^^^^

.. java:constructor:: public MaF04()
   :outertype: MaF04

   Default constructor

MaF04
^^^^^

.. java:constructor:: public MaF04(Integer numberOfVariables, Integer numberOfObjectives)
   :outertype: MaF04

   Creates a MaF04 problem instance

   :param numberOfVariables: Number of variables
   :param numberOfObjectives: Number of objective functions

Methods
-------
evaluate
^^^^^^^^

.. java:method:: @Override public void evaluate(DoubleSolution solution)
   :outertype: MaF04

   Evaluates a solution

   :param solution: The solution to evaluate

