.. java:import:: org.uma.jmetal.problem Problem

.. java:import:: java.io Serializable

.. java:import:: java.util List

SolutionListEvaluator
=====================

.. java:package:: org.uma.jmetal.util.evaluator
   :noindex:

.. java:type:: public interface SolutionListEvaluator<S> extends Serializable

   Created by Antonio J. Nebro on 30/05/14.

Methods
-------
evaluate
^^^^^^^^

.. java:method::  List<S> evaluate(List<S> solutionList, Problem<S> problem)
   :outertype: SolutionListEvaluator

shutdown
^^^^^^^^

.. java:method::  void shutdown()
   :outertype: SolutionListEvaluator

