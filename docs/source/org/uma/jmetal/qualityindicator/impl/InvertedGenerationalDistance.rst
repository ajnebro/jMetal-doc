.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util.front Front

.. java:import:: org.uma.jmetal.util.front.imp ArrayFront

.. java:import:: org.uma.jmetal.util.front.util FrontUtils

.. java:import:: java.io FileNotFoundException

.. java:import:: java.util List

InvertedGenerationalDistance
============================

.. java:package:: org.uma.jmetal.qualityindicator.impl
   :noindex:

.. java:type:: @SuppressWarnings public class InvertedGenerationalDistance<S extends Solution<?>> extends GenericIndicator<S>

   This class implements the inverted generational distance metric. Reference: Van Veldhuizen, D.A., Lamont, G.B.: Multiobjective Evolutionary Algorithm Research: A History and Analysis. Technical Report TR-98-03, Dept. Elec. Comput. Eng., Air Force Inst. Technol. (1998)

   :author: Antonio J. Nebro , Juan J. Durillo

Constructors
------------
InvertedGenerationalDistance
^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public InvertedGenerationalDistance()
   :outertype: InvertedGenerationalDistance

   Default constructor

InvertedGenerationalDistance
^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public InvertedGenerationalDistance(String referenceParetoFrontFile, double p) throws FileNotFoundException
   :outertype: InvertedGenerationalDistance

   Constructor

   :param referenceParetoFrontFile:
   :throws FileNotFoundException:

InvertedGenerationalDistance
^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public InvertedGenerationalDistance(String referenceParetoFrontFile) throws FileNotFoundException
   :outertype: InvertedGenerationalDistance

   Constructor

   :param referenceParetoFrontFile:
   :throws FileNotFoundException:

InvertedGenerationalDistance
^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public InvertedGenerationalDistance(Front referenceParetoFront)
   :outertype: InvertedGenerationalDistance

   Constructor

   :param referenceParetoFront:
   :throws FileNotFoundException:

Methods
-------
evaluate
^^^^^^^^

.. java:method:: @Override public Double evaluate(List<S> solutionList)
   :outertype: InvertedGenerationalDistance

   Evaluate() method

   :param solutionList:

getDescription
^^^^^^^^^^^^^^

.. java:method:: @Override public String getDescription()
   :outertype: InvertedGenerationalDistance

getName
^^^^^^^

.. java:method:: @Override public String getName()
   :outertype: InvertedGenerationalDistance

invertedGenerationalDistance
^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public double invertedGenerationalDistance(Front front, Front referenceFront)
   :outertype: InvertedGenerationalDistance

   Returns the inverted generational distance value for a given front

   :param front: The front
   :param referenceFront: The reference pareto front

isTheLowerTheIndicatorValueTheBetter
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public boolean isTheLowerTheIndicatorValueTheBetter()
   :outertype: InvertedGenerationalDistance

