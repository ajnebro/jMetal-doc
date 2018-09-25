.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: org.uma.jmetal.util.front Front

.. java:import:: org.uma.jmetal.util.front.imp ArrayFront

.. java:import:: java.util List

FrontNormalizer
===============

.. java:package:: org.uma.jmetal.util.front.util
   :noindex:

.. java:type:: public class FrontNormalizer

   Class for normalizing \ :java:ref:`Front`\  objects

   :author: Antonio J. Nebro

Constructors
------------
FrontNormalizer
^^^^^^^^^^^^^^^

.. java:constructor:: public FrontNormalizer(List<? extends Solution<?>> referenceFront)
   :outertype: FrontNormalizer

   Constructor.

   :param referenceFront:

FrontNormalizer
^^^^^^^^^^^^^^^

.. java:constructor:: public FrontNormalizer(Front referenceFront)
   :outertype: FrontNormalizer

   Constructor.

   :param referenceFront:

FrontNormalizer
^^^^^^^^^^^^^^^

.. java:constructor:: public FrontNormalizer(double[] minimumValues, double[] maximumValues)
   :outertype: FrontNormalizer

   Constructor

   :param minimumValues:
   :param maximumValues:

Methods
-------
normalize
^^^^^^^^^

.. java:method:: public List<? extends Solution<?>> normalize(List<? extends Solution<?>> solutionList)
   :outertype: FrontNormalizer

   Returns a normalized front

   :param solutionList:

normalize
^^^^^^^^^

.. java:method:: public Front normalize(Front front)
   :outertype: FrontNormalizer

   Returns a normalized front

   :param front:

