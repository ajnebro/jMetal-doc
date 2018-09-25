ConstrainedProblem
==================

.. java:package:: org.uma.jmetal.problem
   :noindex:

.. java:type:: public interface ConstrainedProblem<S> extends Problem<S>

   Interface representing problems having constraints

   :author: Antonio J. Nebro

Methods
-------
evaluateConstraints
^^^^^^^^^^^^^^^^^^^

.. java:method:: public void evaluateConstraints(S solution)
   :outertype: ConstrainedProblem

getNumberOfConstraints
^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public int getNumberOfConstraints()
   :outertype: ConstrainedProblem

