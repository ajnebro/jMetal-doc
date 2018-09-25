.. java:import:: org.uma.jmetal.problem.impl AbstractDoubleProblem

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: java.util ArrayList

.. java:import:: java.util List

DTLZ5
=====

.. java:package:: org.uma.jmetal.problem.multiobjective.dtlz
   :noindex:

.. java:type:: @SuppressWarnings public class DTLZ5 extends AbstractDoubleProblem

   Class representing problem DTLZ5

Constructors
------------
DTLZ5
^^^^^

.. java:constructor:: public DTLZ5()
   :outertype: DTLZ5

   Creates a default DTLZ5 problem (12 variables and 3 objectives)

DTLZ5
^^^^^

.. java:constructor:: public DTLZ5(Integer numberOfVariables, Integer numberOfObjectives) throws JMetalException
   :outertype: DTLZ5

   Creates a DTLZ5 problem instance

   :param numberOfVariables: Number of variables
   :param numberOfObjectives: Number of objective functions

Methods
-------
evaluate
^^^^^^^^

.. java:method:: public void evaluate(DoubleSolution solution)
   :outertype: DTLZ5

   Evaluate() method

