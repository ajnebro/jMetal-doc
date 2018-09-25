.. java:import:: org.uma.jmetal.problem Problem

.. java:import:: org.uma.jmetal.solution Solution

ExperimentProblem
=================

.. java:package:: org.uma.jmetal.util.experiment.util
   :noindex:

.. java:type:: public class ExperimentProblem<S extends Solution<?>>

   Class used to add a tag field to a problem.

   :author: Antonio J. Nebro

Constructors
------------
ExperimentProblem
^^^^^^^^^^^^^^^^^

.. java:constructor:: public ExperimentProblem(Problem<S> problem, String tag)
   :outertype: ExperimentProblem

ExperimentProblem
^^^^^^^^^^^^^^^^^

.. java:constructor:: public ExperimentProblem(Problem<S> problem)
   :outertype: ExperimentProblem

Methods
-------
changeReferenceFrontTo
^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public ExperimentProblem<S> changeReferenceFrontTo(String referenceFront)
   :outertype: ExperimentProblem

getProblem
^^^^^^^^^^

.. java:method:: public Problem<S> getProblem()
   :outertype: ExperimentProblem

getReferenceFront
^^^^^^^^^^^^^^^^^

.. java:method:: public String getReferenceFront()
   :outertype: ExperimentProblem

getTag
^^^^^^

.. java:method:: public String getTag()
   :outertype: ExperimentProblem

