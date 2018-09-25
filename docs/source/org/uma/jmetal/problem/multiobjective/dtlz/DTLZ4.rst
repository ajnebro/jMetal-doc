.. java:import:: org.uma.jmetal.problem.impl AbstractDoubleProblem

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: java.util ArrayList

.. java:import:: java.util List

DTLZ4
=====

.. java:package:: org.uma.jmetal.problem.multiobjective.dtlz
   :noindex:

.. java:type:: @SuppressWarnings public class DTLZ4 extends AbstractDoubleProblem

   Class representing problem DTLZ4

Constructors
------------
DTLZ4
^^^^^

.. java:constructor:: public DTLZ4()
   :outertype: DTLZ4

   Creates a default DTLZ4 problem (12 variables and 3 objectives)

DTLZ4
^^^^^

.. java:constructor:: public DTLZ4(Integer numberOfVariables, Integer numberOfObjectives) throws JMetalException
   :outertype: DTLZ4

   Creates a DTLZ4 problem instance

   :param numberOfVariables: Number of variables
   :param numberOfObjectives: Number of objective functions

Methods
-------
evaluate
^^^^^^^^

.. java:method:: public void evaluate(DoubleSolution solution)
   :outertype: DTLZ4

   Evaluate() method

