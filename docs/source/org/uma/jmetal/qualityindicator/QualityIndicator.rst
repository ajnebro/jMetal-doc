.. java:import:: org.uma.jmetal.util.naming DescribedEntity

.. java:import:: java.io Serializable

QualityIndicator
================

.. java:package:: org.uma.jmetal.qualityindicator
   :noindex:

.. java:type:: public interface QualityIndicator<Evaluate, Result> extends DescribedEntity, Serializable

   :author: Antonio J. Nebro
   :param <Evaluate>: Entity to runAlgorithm
   :param <Result>: Result of the evaluation

Methods
-------
evaluate
^^^^^^^^

.. java:method:: public Result evaluate(Evaluate evaluate)
   :outertype: QualityIndicator

