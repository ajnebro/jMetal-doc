.. java:import:: org.uma.jmetal.problem ConstrainedProblem

.. java:import:: org.uma.jmetal.problem Problem

.. java:import:: org.uma.jmetal.util JMetalLogger

.. java:import:: org.uma.jmetal.util.evaluator SolutionListEvaluator

.. java:import:: java.util List

MultithreadedSolutionListEvaluator
==================================

.. java:package:: org.uma.jmetal.util.evaluator.impl
   :noindex:

.. java:type:: @SuppressWarnings public class MultithreadedSolutionListEvaluator<S> implements SolutionListEvaluator<S>

   :author: Antonio J. Nebro

Constructors
------------
MultithreadedSolutionListEvaluator
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public MultithreadedSolutionListEvaluator(int numberOfThreads, Problem<S> problem)
   :outertype: MultithreadedSolutionListEvaluator

Methods
-------
evaluate
^^^^^^^^

.. java:method:: @Override public List<S> evaluate(List<S> solutionList, Problem<S> problem)
   :outertype: MultithreadedSolutionListEvaluator

getNumberOfThreads
^^^^^^^^^^^^^^^^^^

.. java:method:: public int getNumberOfThreads()
   :outertype: MultithreadedSolutionListEvaluator

shutdown
^^^^^^^^

.. java:method:: @Override public void shutdown()
   :outertype: MultithreadedSolutionListEvaluator

