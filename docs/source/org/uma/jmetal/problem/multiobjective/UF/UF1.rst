.. java:import:: org.uma.jmetal.problem.impl AbstractDoubleProblem

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: java.util ArrayList

.. java:import:: java.util List

UF1
===

.. java:package:: org.uma.jmetal.problem.multiobjective.UF
   :noindex:

.. java:type:: @SuppressWarnings public class UF1 extends AbstractDoubleProblem

   Class representing problem CEC2009_UF1

Constructors
------------
UF1
^^^

.. java:constructor:: public UF1()
   :outertype: UF1

   Constructor. Creates a default instance of problem CEC2009_UF1 (30 decision variables)

UF1
^^^

.. java:constructor:: public UF1(int numberOfVariables)
   :outertype: UF1

   Creates a new instance of problem CEC2009_UF1.

   :param numberOfVariables: Number of variables.

Methods
-------
evaluate
^^^^^^^^

.. java:method:: @Override public void evaluate(DoubleSolution solution)
   :outertype: UF1

   Evaluate() method

