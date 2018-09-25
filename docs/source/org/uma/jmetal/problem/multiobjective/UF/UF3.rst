.. java:import:: org.uma.jmetal.problem.impl AbstractDoubleProblem

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: java.util ArrayList

.. java:import:: java.util List

UF3
===

.. java:package:: org.uma.jmetal.problem.multiobjective.UF
   :noindex:

.. java:type:: @SuppressWarnings public class UF3 extends AbstractDoubleProblem

   Class representing problem CEC2009_UF3

Constructors
------------
UF3
^^^

.. java:constructor:: public UF3()
   :outertype: UF3

   Constructor. Creates a default instance of problem CEC2009_UF3 (30 decision variables)

UF3
^^^

.. java:constructor:: public UF3(int numberOfVariables)
   :outertype: UF3

   Creates a new instance of problem CEC2009_UF3.

   :param numberOfVariables: Number of variables.

Methods
-------
evaluate
^^^^^^^^

.. java:method:: @Override public void evaluate(DoubleSolution solution)
   :outertype: UF3

   Evaluate() method

