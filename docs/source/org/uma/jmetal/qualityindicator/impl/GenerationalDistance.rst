.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: org.uma.jmetal.util.front Front

.. java:import:: org.uma.jmetal.util.front.imp ArrayFront

.. java:import:: org.uma.jmetal.util.front.util FrontUtils

.. java:import:: java.io FileNotFoundException

.. java:import:: java.util List

GenerationalDistance
====================

.. java:package:: org.uma.jmetal.qualityindicator.impl
   :noindex:

.. java:type:: @SuppressWarnings public class GenerationalDistance<S extends Solution<?>> extends GenericIndicator<S>

   This class implements the generational distance indicator. Reference: Van Veldhuizen, D.A., Lamont, G.B.: Multiobjective Evolutionary Algorithm Research: A History and Analysis. Technical Report TR-98-03, Dept. Elec. Comput. Eng., Air Force Inst. Technol. (1998)

   :author: Antonio J. Nebro , Juan J. Durillo

Constructors
------------
GenerationalDistance
^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public GenerationalDistance()
   :outertype: GenerationalDistance

   Default constructor

GenerationalDistance
^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public GenerationalDistance(String referenceParetoFrontFile, double p) throws FileNotFoundException
   :outertype: GenerationalDistance

   Constructor

   :param referenceParetoFrontFile:
   :param p:
   :throws FileNotFoundException:

GenerationalDistance
^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public GenerationalDistance(String referenceParetoFrontFile) throws FileNotFoundException
   :outertype: GenerationalDistance

   Constructor

   :param referenceParetoFrontFile:
   :throws FileNotFoundException:

GenerationalDistance
^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public GenerationalDistance(Front referenceParetoFront)
   :outertype: GenerationalDistance

   Constructor

   :param referenceParetoFront:

Methods
-------
evaluate
^^^^^^^^

.. java:method:: @Override public Double evaluate(List<S> solutionList)
   :outertype: GenerationalDistance

   Evaluate() method

   :param solutionList:

generationalDistance
^^^^^^^^^^^^^^^^^^^^

.. java:method:: public double generationalDistance(Front front, Front referenceFront)
   :outertype: GenerationalDistance

   Returns the generational distance value for a given front

   :param front: The front
   :param referenceFront: The reference pareto front

getDescription
^^^^^^^^^^^^^^

.. java:method:: @Override public String getDescription()
   :outertype: GenerationalDistance

getName
^^^^^^^

.. java:method:: @Override public String getName()
   :outertype: GenerationalDistance

isTheLowerTheIndicatorValueTheBetter
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public boolean isTheLowerTheIndicatorValueTheBetter()
   :outertype: GenerationalDistance

