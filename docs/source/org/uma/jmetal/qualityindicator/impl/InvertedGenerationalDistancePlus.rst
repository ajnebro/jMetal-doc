.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: org.uma.jmetal.util.front Front

.. java:import:: org.uma.jmetal.util.front.imp ArrayFront

.. java:import:: org.uma.jmetal.util.front.util FrontUtils

.. java:import:: org.uma.jmetal.util.point.util.distance DominanceDistance

.. java:import:: java.io FileNotFoundException

.. java:import:: java.util List

InvertedGenerationalDistancePlus
================================

.. java:package:: org.uma.jmetal.qualityindicator.impl
   :noindex:

.. java:type:: @SuppressWarnings public class InvertedGenerationalDistancePlus<S extends Solution<?>> extends GenericIndicator<S>

   This class implements the inverted generational distance metric plust (IGD+) Reference: Ishibuchi et al 2015, "A Study on Performance Evaluation Ability of a Modified Inverted Generational Distance Indicator", GECCO 2015

   :author: Antonio J. Nebro

Constructors
------------
InvertedGenerationalDistancePlus
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public InvertedGenerationalDistancePlus()
   :outertype: InvertedGenerationalDistancePlus

   Default constructor

InvertedGenerationalDistancePlus
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public InvertedGenerationalDistancePlus(String referenceParetoFrontFile) throws FileNotFoundException
   :outertype: InvertedGenerationalDistancePlus

   Constructor

   :param referenceParetoFrontFile:

InvertedGenerationalDistancePlus
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public InvertedGenerationalDistancePlus(Front referenceParetoFront)
   :outertype: InvertedGenerationalDistancePlus

   Constructor

   :param referenceParetoFront:
   :throws FileNotFoundException:

Methods
-------
evaluate
^^^^^^^^

.. java:method:: @Override public Double evaluate(List<S> solutionList)
   :outertype: InvertedGenerationalDistancePlus

   Evaluate() method

   :param solutionList:

getDescription
^^^^^^^^^^^^^^

.. java:method:: @Override public String getDescription()
   :outertype: InvertedGenerationalDistancePlus

getName
^^^^^^^

.. java:method:: @Override public String getName()
   :outertype: InvertedGenerationalDistancePlus

invertedGenerationalDistancePlus
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public double invertedGenerationalDistancePlus(Front front, Front referenceFront)
   :outertype: InvertedGenerationalDistancePlus

   Returns the inverted generational distance plus value for a given front

   :param front: The front
   :param referenceFront: The reference pareto front

isTheLowerTheIndicatorValueTheBetter
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public boolean isTheLowerTheIndicatorValueTheBetter()
   :outertype: InvertedGenerationalDistancePlus

