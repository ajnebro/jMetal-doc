.. java:import:: org.uma.jmetal.problem.impl AbstractDoubleProblem

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: java.util ArrayList

.. java:import:: java.util List

DTLZ6
=====

.. java:package:: org.uma.jmetal.problem.multiobjective.dtlz
   :noindex:

.. java:type:: @SuppressWarnings public class DTLZ6 extends AbstractDoubleProblem

   Class representing problem DTLZ6

Constructors
------------
DTLZ6
^^^^^

.. java:constructor:: public DTLZ6()
   :outertype: DTLZ6

   Creates a default DTLZ6 problem (12 variables and 3 objectives)

DTLZ6
^^^^^

.. java:constructor:: public DTLZ6(Integer numberOfVariables, Integer numberOfObjectives) throws JMetalException
   :outertype: DTLZ6

   Creates a DTLZ6 problem instance

   :param numberOfVariables: Number of variables
   :param numberOfObjectives: Number of objective functions

Methods
-------
evaluate
^^^^^^^^

.. java:method:: public void evaluate(DoubleSolution solution)
   :outertype: DTLZ6

   Evaluate() method

