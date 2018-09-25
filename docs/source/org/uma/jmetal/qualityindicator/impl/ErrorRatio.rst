.. java:import:: org.uma.jmetal.qualityindicator QualityIndicator

.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: org.uma.jmetal.util.front Front

.. java:import:: org.uma.jmetal.util.front.imp ArrayFront

.. java:import:: org.uma.jmetal.util.naming.impl SimpleDescribedEntity

.. java:import:: org.uma.jmetal.util.point Point

.. java:import:: java.io FileNotFoundException

.. java:import:: java.util List

ErrorRatio
==========

.. java:package:: org.uma.jmetal.qualityindicator.impl
   :noindex:

.. java:type:: @SuppressWarnings public class ErrorRatio<Evaluate extends List<? extends Solution<?>>> extends SimpleDescribedEntity implements QualityIndicator<Evaluate, Double>

   The Error Ratio (ER) quality indicator reports the ratio of solutions in a front of points that are not members of the true Pareto front. NOTE: the indicator merely checks if the solutions in the front are not members of the second front. No assumption is made about the second front is a true Pareto front, i.e, the front could contain solutions that dominate some of those of the supposed Pareto front. It is a responsibility of the caller to ensure that this does not happen.

   :author: Antonio J. Nebro  TODO: using an epsilon value

Constructors
------------
ErrorRatio
^^^^^^^^^^

.. java:constructor:: public ErrorRatio(String referenceParetoFrontFile) throws FileNotFoundException
   :outertype: ErrorRatio

   Constructor

   :param referenceParetoFrontFile:
   :throws FileNotFoundException:

ErrorRatio
^^^^^^^^^^

.. java:constructor:: public ErrorRatio(Front referenceParetoFront)
   :outertype: ErrorRatio

   Constructor

   :param referenceParetoFront:

Methods
-------
evaluate
^^^^^^^^

.. java:method:: @Override public Double evaluate(Evaluate solutionList)
   :outertype: ErrorRatio

   Evaluate() method

   :param solutionList:

getName
^^^^^^^

.. java:method:: @Override public String getName()
   :outertype: ErrorRatio

