.. java:import:: org.uma.jmetal.qualityindicator QualityIndicator

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: org.uma.jmetal.util.front Front

.. java:import:: org.uma.jmetal.util.front.imp ArrayFront

.. java:import:: org.uma.jmetal.util.naming.impl SimpleDescribedEntity

.. java:import:: java.io FileNotFoundException

.. java:import:: java.util List

GenericIndicator
================

.. java:package:: org.uma.jmetal.qualityindicator.impl
   :noindex:

.. java:type:: @SuppressWarnings public abstract class GenericIndicator<S> extends SimpleDescribedEntity implements QualityIndicator<List<S>, Double>

   Abstract class representing quality indicators that need a reference front to be computed

   :author: Antonio J. Nebro

Fields
------
referenceParetoFront
^^^^^^^^^^^^^^^^^^^^

.. java:field:: protected Front referenceParetoFront
   :outertype: GenericIndicator

Constructors
------------
GenericIndicator
^^^^^^^^^^^^^^^^

.. java:constructor:: public GenericIndicator()
   :outertype: GenericIndicator

   Default constructor

GenericIndicator
^^^^^^^^^^^^^^^^

.. java:constructor:: public GenericIndicator(String referenceParetoFrontFile) throws FileNotFoundException
   :outertype: GenericIndicator

GenericIndicator
^^^^^^^^^^^^^^^^

.. java:constructor:: public GenericIndicator(Front referenceParetoFront)
   :outertype: GenericIndicator

Methods
-------
isTheLowerTheIndicatorValueTheBetter
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public abstract boolean isTheLowerTheIndicatorValueTheBetter()
   :outertype: GenericIndicator

   This method returns true if lower indicator values are preferred and false otherwise

setReferenceParetoFront
^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public void setReferenceParetoFront(String referenceParetoFrontFile) throws FileNotFoundException
   :outertype: GenericIndicator

setReferenceParetoFront
^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public void setReferenceParetoFront(Front referenceFront) throws FileNotFoundException
   :outertype: GenericIndicator

