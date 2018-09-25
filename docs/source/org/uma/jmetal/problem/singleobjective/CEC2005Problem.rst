.. java:import:: org.uma.jmetal.problem.impl AbstractDoubleProblem

.. java:import:: org.uma.jmetal.problem.singleobjective.cec2005competitioncode Benchmark

.. java:import:: org.uma.jmetal.problem.singleobjective.cec2005competitioncode TestFunc

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: java.util ArrayList

.. java:import:: java.util List

CEC2005Problem
==============

.. java:package:: org.uma.jmetal.problem.singleobjective
   :noindex:

.. java:type:: @SuppressWarnings public class CEC2005Problem extends AbstractDoubleProblem

   Class representing for solving the CEC2005 competition problems.

Fields
------
testFunction
^^^^^^^^^^^^

.. java:field::  TestFunc testFunction
   :outertype: CEC2005Problem

Constructors
------------
CEC2005Problem
^^^^^^^^^^^^^^

.. java:constructor:: public CEC2005Problem(int problemID, int numberOfVariables)
   :outertype: CEC2005Problem

   Constructor

Methods
-------
evaluate
^^^^^^^^

.. java:method:: @Override public void evaluate(DoubleSolution solution)
   :outertype: CEC2005Problem

   Evaluate() method

