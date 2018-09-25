.. java:import:: org.uma.jmetal.problem.impl AbstractDoubleProblem

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: java.util ArrayList

.. java:import:: java.util List

UF4
===

.. java:package:: org.uma.jmetal.problem.multiobjective.UF
   :noindex:

.. java:type:: @SuppressWarnings public class UF4 extends AbstractDoubleProblem

   Class representing problem CEC2009_UF4

Constructors
------------
UF4
^^^

.. java:constructor:: public UF4()
   :outertype: UF4

   Constructor. Creates a default instance of problem CEC2009_UF4 (30 decision variables)

UF4
^^^

.. java:constructor:: public UF4(Integer numberOfVariables)
   :outertype: UF4

   Creates a new instance of problem CEC2009_UF4.

   :param numberOfVariables: Number of variables.

Methods
-------
evaluate
^^^^^^^^

.. java:method:: @Override public void evaluate(DoubleSolution solution)
   :outertype: UF4

   Evaluate() method

