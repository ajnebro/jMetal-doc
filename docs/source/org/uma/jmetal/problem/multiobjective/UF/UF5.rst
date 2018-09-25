.. java:import:: org.uma.jmetal.problem.impl AbstractDoubleProblem

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: java.util ArrayList

.. java:import:: java.util List

UF5
===

.. java:package:: org.uma.jmetal.problem.multiobjective.UF
   :noindex:

.. java:type:: @SuppressWarnings public class UF5 extends AbstractDoubleProblem

   Class representing problem CEC2009_UF5

Fields
------
epsilon
^^^^^^^

.. java:field::  double epsilon
   :outertype: UF5

n
^

.. java:field::  int n
   :outertype: UF5

Constructors
------------
UF5
^^^

.. java:constructor:: public UF5()
   :outertype: UF5

   Constructor. Creates a default instance of problem CEC2009_UF5 (30 decision variables)

UF5
^^^

.. java:constructor:: public UF5(int numberOfVariables, int N, double epsilon)
   :outertype: UF5

   Creates a new instance of problem CEC2009_UF5.

   :param numberOfVariables: Number of variables.

Methods
-------
evaluate
^^^^^^^^

.. java:method:: @Override public void evaluate(DoubleSolution solution)
   :outertype: UF5

   Evaluate() method

