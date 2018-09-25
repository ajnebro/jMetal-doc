.. java:import:: org.uma.jmetal.problem.impl AbstractDoubleProblem

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: java.util ArrayList

.. java:import:: java.util List

UF2
===

.. java:package:: org.uma.jmetal.problem.multiobjective.UF
   :noindex:

.. java:type:: @SuppressWarnings public class UF2 extends AbstractDoubleProblem

   Class representing problem CEC2009_UF2

Constructors
------------
UF2
^^^

.. java:constructor:: public UF2()
   :outertype: UF2

   Constructor. Creates a default instance of problem CEC2009_UF2 (30 decision variables)

UF2
^^^

.. java:constructor:: public UF2(int numberOfVariables)
   :outertype: UF2

   Creates a new instance of problem CEC2009_UF2.

   :param numberOfVariables: Number of variables.

Methods
-------
evaluate
^^^^^^^^

.. java:method:: @Override public void evaluate(DoubleSolution solution)
   :outertype: UF2

   Evaluate() method

