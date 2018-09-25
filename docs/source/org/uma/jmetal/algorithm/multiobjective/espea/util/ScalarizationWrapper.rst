.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: java.util List

ScalarizationWrapper
====================

.. java:package:: org.uma.jmetal.algorithm.multiobjective.espea.util
   :noindex:

.. java:type:: public class ScalarizationWrapper

   A class for simplifying the access to \ :java:ref:`ScalarizationUtils`\ .

   :author: Marlon Braun

Constructors
------------
ScalarizationWrapper
^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public ScalarizationWrapper(ScalarizationType scalarizationType)
   :outertype: ScalarizationWrapper

   Initialize from scalarization type

   :param scalarizationType: Chosen scalarization function

ScalarizationWrapper
^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public ScalarizationWrapper(Config config)
   :outertype: ScalarizationWrapper

   Initialize from Config.

   :param config: Configuration of the scalarization Wrapper.

Methods
-------
execute
^^^^^^^

.. java:method:: public <S extends Solution<?>> void execute(List<S> solutionsList)
   :outertype: ScalarizationWrapper

   Computes scalarization values and assigns them as \ :java:ref:`ScalarizationValue`\  attribute to the solutions.

   :param solutionsList: Solutions for which scalarization values computed.

