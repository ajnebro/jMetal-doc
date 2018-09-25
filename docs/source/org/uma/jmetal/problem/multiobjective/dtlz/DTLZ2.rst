.. java:import:: org.uma.jmetal.problem.impl AbstractDoubleProblem

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: java.util ArrayList

.. java:import:: java.util List

DTLZ2
=====

.. java:package:: org.uma.jmetal.problem.multiobjective.dtlz
   :noindex:

.. java:type:: @SuppressWarnings public class DTLZ2 extends AbstractDoubleProblem

   Class representing problem DTLZ1

Constructors
------------
DTLZ2
^^^^^

.. java:constructor:: public DTLZ2()
   :outertype: DTLZ2

   Creates a default DTLZ2 problem (12 variables and 3 objectives)

DTLZ2
^^^^^

.. java:constructor:: public DTLZ2(Integer numberOfVariables, Integer numberOfObjectives) throws JMetalException
   :outertype: DTLZ2

   Creates a DTLZ2 problem instance

   :param numberOfVariables: Number of variables
   :param numberOfObjectives: Number of objective functions

Methods
-------
evaluate
^^^^^^^^

.. java:method:: public void evaluate(DoubleSolution solution)
   :outertype: DTLZ2

   Evaluate() method

