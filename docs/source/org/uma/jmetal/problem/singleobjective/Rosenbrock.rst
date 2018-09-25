.. java:import:: org.uma.jmetal.problem.impl AbstractDoubleProblem

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: java.util ArrayList

.. java:import:: java.util List

Rosenbrock
==========

.. java:package:: org.uma.jmetal.problem.singleobjective
   :noindex:

.. java:type:: @SuppressWarnings public class Rosenbrock extends AbstractDoubleProblem

Constructors
------------
Rosenbrock
^^^^^^^^^^

.. java:constructor:: public Rosenbrock(Integer numberOfVariables)
   :outertype: Rosenbrock

   Constructor Creates a default instance of the Rosenbrock problem

   :param numberOfVariables: Number of variables of the problem

Methods
-------
evaluate
^^^^^^^^

.. java:method:: @Override public void evaluate(DoubleSolution solution)
   :outertype: Rosenbrock

   Evaluate() method

