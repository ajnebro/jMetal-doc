.. java:import:: org.uma.jmetal.problem.impl AbstractDoubleProblem

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: java.util ArrayList

.. java:import:: java.util List

Griewank
========

.. java:package:: org.uma.jmetal.problem.singleobjective
   :noindex:

.. java:type:: @SuppressWarnings public class Griewank extends AbstractDoubleProblem

   Class representing problem Griewank

Constructors
------------
Griewank
^^^^^^^^

.. java:constructor:: public Griewank(Integer numberOfVariables)
   :outertype: Griewank

   Constructor Creates a default instance of the Griewank problem

   :param numberOfVariables: Number of variables of the problem

Methods
-------
evaluate
^^^^^^^^

.. java:method:: @Override public void evaluate(DoubleSolution solution)
   :outertype: Griewank

   Evaluate() method

