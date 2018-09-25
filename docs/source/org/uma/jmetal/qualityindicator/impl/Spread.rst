.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util.front Front

.. java:import:: org.uma.jmetal.util.front.imp ArrayFront

.. java:import:: org.uma.jmetal.util.point.util.comparator LexicographicalPointComparator

.. java:import:: org.uma.jmetal.util.point.util.distance EuclideanDistance

.. java:import:: org.uma.jmetal.util.point.util.distance PointDistance

.. java:import:: java.io FileNotFoundException

.. java:import:: java.util List

Spread
======

.. java:package:: org.uma.jmetal.qualityindicator.impl
   :noindex:

.. java:type:: @SuppressWarnings public class Spread<S extends Solution<?>> extends GenericIndicator<S>

   This class implements the spread quality indicator. It must be only to two bi-objective problem. Reference: Deb, K., Pratap, A., Agarwal, S., Meyarivan, T.: A fast and elitist multiobjective genetic algorithm: NSGA-II. IEEE Trans. on Evol. Computation 6 (2002) 182-197

   :author: Antonio J. Nebro , Juan J. Durillo

Constructors
------------
Spread
^^^^^^

.. java:constructor:: public Spread()
   :outertype: Spread

   Default constructor

Spread
^^^^^^

.. java:constructor:: public Spread(String referenceParetoFrontFile) throws FileNotFoundException
   :outertype: Spread

   Constructor

   :param referenceParetoFrontFile:
   :throws FileNotFoundException:

Spread
^^^^^^

.. java:constructor:: public Spread(Front referenceParetoFront)
   :outertype: Spread

   Constructor

   :param referenceParetoFront:
   :throws FileNotFoundException:

Methods
-------
evaluate
^^^^^^^^

.. java:method:: @Override public Double evaluate(List<S> solutionList)
   :outertype: Spread

   Evaluate() method

   :param solutionList:

getDescription
^^^^^^^^^^^^^^

.. java:method:: @Override public String getDescription()
   :outertype: Spread

getName
^^^^^^^

.. java:method:: @Override public String getName()
   :outertype: Spread

isTheLowerTheIndicatorValueTheBetter
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public boolean isTheLowerTheIndicatorValueTheBetter()
   :outertype: Spread

spread
^^^^^^

.. java:method:: public double spread(Front front, Front referenceFront)
   :outertype: Spread

   Calculates the Spread metric.

   :param front: The front.
   :param referenceFront: The true pareto front.

