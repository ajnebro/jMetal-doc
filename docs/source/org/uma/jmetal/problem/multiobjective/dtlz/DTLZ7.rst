.. java:import:: org.uma.jmetal.problem.impl AbstractDoubleProblem

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: java.util ArrayList

.. java:import:: java.util List

DTLZ7
=====

.. java:package:: org.uma.jmetal.problem.multiobjective.dtlz
   :noindex:

.. java:type:: @SuppressWarnings public class DTLZ7 extends AbstractDoubleProblem

   Class representing problem DTLZ7

Constructors
------------
DTLZ7
^^^^^

.. java:constructor:: public DTLZ7()
   :outertype: DTLZ7

   Creates a default DTLZ7 problem (22 variables and 3 objectives)

DTLZ7
^^^^^

.. java:constructor:: public DTLZ7(Integer numberOfVariables, Integer numberOfObjectives) throws JMetalException
   :outertype: DTLZ7

   Creates a DTLZ7 problem instance

   :param numberOfVariables: Number of variables
   :param numberOfObjectives: Number of objective functions

Methods
-------
evaluate
^^^^^^^^

.. java:method:: public void evaluate(DoubleSolution solution)
   :outertype: DTLZ7

   Evaluate() method

