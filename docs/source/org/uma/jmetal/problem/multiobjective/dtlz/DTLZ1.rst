.. java:import:: org.uma.jmetal.problem.impl AbstractDoubleProblem

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: java.util ArrayList

.. java:import:: java.util List

DTLZ1
=====

.. java:package:: org.uma.jmetal.problem.multiobjective.dtlz
   :noindex:

.. java:type:: @SuppressWarnings public class DTLZ1 extends AbstractDoubleProblem

   Class representing problem DTLZ1

Constructors
------------
DTLZ1
^^^^^

.. java:constructor:: public DTLZ1()
   :outertype: DTLZ1

   Creates a default DTLZ1 problem (7 variables and 3 objectives)

DTLZ1
^^^^^

.. java:constructor:: public DTLZ1(Integer numberOfVariables, Integer numberOfObjectives) throws JMetalException
   :outertype: DTLZ1

   Creates a DTLZ1 problem instance

   :param numberOfVariables: Number of variables
   :param numberOfObjectives: Number of objective functions

Methods
-------
evaluate
^^^^^^^^

.. java:method:: public void evaluate(DoubleSolution solution)
   :outertype: DTLZ1

   Evaluate() method

