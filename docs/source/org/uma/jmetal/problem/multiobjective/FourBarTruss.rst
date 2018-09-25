.. java:import:: org.uma.jmetal.problem.impl AbstractDoubleProblem

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: java.util ArrayList

.. java:import:: java.util List

FourBarTruss
============

.. java:package:: org.uma.jmetal.problem.multiobjective
   :noindex:

.. java:type:: @SuppressWarnings public class FourBarTruss extends AbstractDoubleProblem

   Class representing problem FourBarTruss Measures: f = 10kN e = 200000 kN/cm2 l = 200 cm sigma = 10kN/cm2

Constructors
------------
FourBarTruss
^^^^^^^^^^^^

.. java:constructor:: public FourBarTruss()
   :outertype: FourBarTruss

   Constructor Creates a default instance of the FourBarTruss problem

Methods
-------
evaluate
^^^^^^^^

.. java:method:: @Override public void evaluate(DoubleSolution solution)
   :outertype: FourBarTruss

   Evaluate() method

