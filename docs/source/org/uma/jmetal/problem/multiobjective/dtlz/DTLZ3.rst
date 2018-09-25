.. java:import:: org.uma.jmetal.problem.impl AbstractDoubleProblem

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: java.util ArrayList

.. java:import:: java.util List

DTLZ3
=====

.. java:package:: org.uma.jmetal.problem.multiobjective.dtlz
   :noindex:

.. java:type:: @SuppressWarnings public class DTLZ3 extends AbstractDoubleProblem

   Class representing problem DTLZ3

Constructors
------------
DTLZ3
^^^^^

.. java:constructor:: public DTLZ3()
   :outertype: DTLZ3

   Creates a default DTLZ3 problem (12 variables and 3 objectives)

DTLZ3
^^^^^

.. java:constructor:: public DTLZ3(Integer numberOfVariables, Integer numberOfObjectives) throws JMetalException
   :outertype: DTLZ3

   Creates a DTLZ3 problem instance

   :param numberOfVariables: Number of variables
   :param numberOfObjectives: Number of objective functions

Methods
-------
evaluate
^^^^^^^^

.. java:method:: public void evaluate(DoubleSolution solution)
   :outertype: DTLZ3

   Evaluate() method

