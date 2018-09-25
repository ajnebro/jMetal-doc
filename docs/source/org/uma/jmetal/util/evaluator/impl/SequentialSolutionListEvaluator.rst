.. java:import:: org.uma.jmetal.problem ConstrainedProblem

.. java:import:: org.uma.jmetal.problem Problem

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: org.uma.jmetal.util.evaluator SolutionListEvaluator

.. java:import:: java.util List

SequentialSolutionListEvaluator
===============================

.. java:package:: org.uma.jmetal.util.evaluator.impl
   :noindex:

.. java:type:: @SuppressWarnings public class SequentialSolutionListEvaluator<S> implements SolutionListEvaluator<S>

   :author: Antonio J. Nebro

Methods
-------
evaluate
^^^^^^^^

.. java:method:: @Override public List<S> evaluate(List<S> solutionList, Problem<S> problem) throws JMetalException
   :outertype: SequentialSolutionListEvaluator

shutdown
^^^^^^^^

.. java:method:: @Override public void shutdown()
   :outertype: SequentialSolutionListEvaluator

