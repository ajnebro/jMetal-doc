.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util.front Front

.. java:import:: org.uma.jmetal.util.front.imp ArrayFront

.. java:import:: org.uma.jmetal.util.front.util FrontUtils

.. java:import:: org.uma.jmetal.util.point Point

.. java:import:: org.uma.jmetal.util.point.impl ArrayPoint

.. java:import:: org.uma.jmetal.util.point.util.comparator LexicographicalPointComparator

.. java:import:: org.uma.jmetal.util.point.util.comparator PointDimensionComparator

.. java:import:: org.uma.jmetal.util.point.util.distance EuclideanDistance

.. java:import:: java.io FileNotFoundException

.. java:import:: java.util List

GeneralizedSpread
=================

.. java:package:: org.uma.jmetal.qualityindicator.impl
   :noindex:

.. java:type:: @SuppressWarnings public class GeneralizedSpread<S extends Solution<?>> extends GenericIndicator<S>

   This class implements the generalized spread metric for two or more dimensions. Reference: A. Zhou, Y. Jin, Q. Zhang, B. Sendhoff, and E. Tsang Combining model-based and genetics-based offspring generation for multi-objective optimization using a convergence criterion, 2006 IEEE Congress on Evolutionary Computation, 2006, pp. 3234-3241.

   :author: Antonio J. Nebro , Juan J. Durillo

Constructors
------------
GeneralizedSpread
^^^^^^^^^^^^^^^^^

.. java:constructor:: public GeneralizedSpread()
   :outertype: GeneralizedSpread

   Default constructor

GeneralizedSpread
^^^^^^^^^^^^^^^^^

.. java:constructor:: public GeneralizedSpread(String referenceParetoFrontFile) throws FileNotFoundException
   :outertype: GeneralizedSpread

   Constructor

   :param referenceParetoFrontFile:
   :throws FileNotFoundException:

GeneralizedSpread
^^^^^^^^^^^^^^^^^

.. java:constructor:: public GeneralizedSpread(Front referenceParetoFront)
   :outertype: GeneralizedSpread

   Constructor

   :param referenceParetoFront:
   :throws FileNotFoundException:

Methods
-------
evaluate
^^^^^^^^

.. java:method:: @Override public Double evaluate(List<S> solutionList)
   :outertype: GeneralizedSpread

   Evaluate() method

   :param solutionList:

generalizedSpread
^^^^^^^^^^^^^^^^^

.. java:method:: public double generalizedSpread(Front front, Front referenceFront)
   :outertype: GeneralizedSpread

   Calculates the generalized spread metric. Given the pareto front, the true pareto front as \ ``double []``\  and the number of objectives, the method return the value for the metric.

   :param front: The front.
   :param referenceFront: The reference pareto front.
   :return: the value of the generalized spread metric

getDescription
^^^^^^^^^^^^^^

.. java:method:: @Override public String getDescription()
   :outertype: GeneralizedSpread

getName
^^^^^^^

.. java:method:: @Override public String getName()
   :outertype: GeneralizedSpread

isTheLowerTheIndicatorValueTheBetter
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public boolean isTheLowerTheIndicatorValueTheBetter()
   :outertype: GeneralizedSpread

