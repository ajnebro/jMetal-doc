.. java:import:: org.uma.jmetal.problem.impl AbstractDoubleProblem

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: java.util ArrayList

.. java:import:: java.util List

UF7
===

.. java:package:: org.uma.jmetal.problem.multiobjective.UF
   :noindex:

.. java:type:: @SuppressWarnings public class UF7 extends AbstractDoubleProblem

   Class representing problem CEC2009_UF7

Constructors
------------
UF7
^^^

.. java:constructor:: public UF7()
   :outertype: UF7

   Constructor. Creates a default instance of problem CEC2009_UF7 (30 decision variables)

UF7
^^^

.. java:constructor:: public UF7(int numberOfVariables)
   :outertype: UF7

   Creates a new instance of problem CEC2009_UF7.

   :param numberOfVariables: Number of variables.

Methods
-------
evaluate
^^^^^^^^

.. java:method:: @Override public void evaluate(DoubleSolution solution)
   :outertype: UF7

   Evaluate() method

