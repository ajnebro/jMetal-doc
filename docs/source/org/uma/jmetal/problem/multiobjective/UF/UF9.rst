.. java:import:: org.uma.jmetal.problem.impl AbstractDoubleProblem

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: java.util ArrayList

.. java:import:: java.util List

UF9
===

.. java:package:: org.uma.jmetal.problem.multiobjective.UF
   :noindex:

.. java:type:: @SuppressWarnings public class UF9 extends AbstractDoubleProblem

   Class representing problem CEC2009_UF9

Fields
------
epsilon
^^^^^^^

.. java:field::  double epsilon
   :outertype: UF9

Constructors
------------
UF9
^^^

.. java:constructor:: public UF9()
   :outertype: UF9

   Constructor. Creates a default instance of problem CEC2009_UF9 (30 decision variables, epsilon = 0.1)

UF9
^^^

.. java:constructor:: public UF9(int numberOfVariables, double epsilon)
   :outertype: UF9

   Creates a new instance of problem CEC2009_UF9.

   :param numberOfVariables: Number of variables.

Methods
-------
evaluate
^^^^^^^^

.. java:method:: @Override public void evaluate(DoubleSolution solution)
   :outertype: UF9

   Evaluate() method

