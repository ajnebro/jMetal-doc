.. java:import:: org.uma.jmetal.problem.impl AbstractDoubleProblem

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: java.util ArrayList

.. java:import:: java.util List

UF6
===

.. java:package:: org.uma.jmetal.problem.multiobjective.UF
   :noindex:

.. java:type:: @SuppressWarnings public class UF6 extends AbstractDoubleProblem

   Class representing problem CEC2009_UF5

Fields
------
epsilon
^^^^^^^

.. java:field::  double epsilon
   :outertype: UF6

n
^

.. java:field::  int n
   :outertype: UF6

Constructors
------------
UF6
^^^

.. java:constructor:: public UF6()
   :outertype: UF6

   Constructor. Creates a default instance of problem CEC2009_UF6 (30 decision variables, N =10, epsilon = 0.1)

UF6
^^^

.. java:constructor:: public UF6(Integer numberOfVariables, int N, double epsilon)
   :outertype: UF6

   Creates a new instance of problem CEC2009_UF6.

   :param numberOfVariables: Number of variables.

Methods
-------
evaluate
^^^^^^^^

.. java:method:: @Override public void evaluate(DoubleSolution solution)
   :outertype: UF6

   Evaluate() method

