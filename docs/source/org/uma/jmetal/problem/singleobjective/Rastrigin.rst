.. java:import:: org.uma.jmetal.problem.impl AbstractDoubleProblem

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: java.util ArrayList

.. java:import:: java.util List

Rastrigin
=========

.. java:package:: org.uma.jmetal.problem.singleobjective
   :noindex:

.. java:type:: @SuppressWarnings public class Rastrigin extends AbstractDoubleProblem

Constructors
------------
Rastrigin
^^^^^^^^^

.. java:constructor:: public Rastrigin(Integer numberOfVariables)
   :outertype: Rastrigin

   Constructor Creates a default instance of the Rastrigin problem

   :param numberOfVariables: Number of variables of the problem

Methods
-------
evaluate
^^^^^^^^

.. java:method:: @Override public void evaluate(DoubleSolution solution)
   :outertype: Rastrigin

   Evaluate() method

