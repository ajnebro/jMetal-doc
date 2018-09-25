.. java:import:: org.uma.jmetal.problem.impl AbstractDoubleProblem

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: java.util ArrayList

.. java:import:: java.util List

UF8
===

.. java:package:: org.uma.jmetal.problem.multiobjective.UF
   :noindex:

.. java:type:: @SuppressWarnings public class UF8 extends AbstractDoubleProblem

   Class representing problem CEC2009_UF8

Constructors
------------
UF8
^^^

.. java:constructor:: public UF8()
   :outertype: UF8

   Constructor. Creates a default instance of problem CEC2009_UF8 (30 decision variables)

UF8
^^^

.. java:constructor:: public UF8(int numberOfVariables)
   :outertype: UF8

   Creates a new instance of problem CEC2009_UF8.

   :param numberOfVariables: Number of variables.

Methods
-------
evaluate
^^^^^^^^

.. java:method:: @Override public void evaluate(DoubleSolution solution)
   :outertype: UF8

   Evaluate() method

