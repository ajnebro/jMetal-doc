.. java:import:: org.uma.jmetal.util.front Front

.. java:import:: java.io FileNotFoundException

.. java:import:: java.util List

Hypervolume
===========

.. java:package:: org.uma.jmetal.qualityindicator.impl
   :noindex:

.. java:type:: @SuppressWarnings public abstract class Hypervolume<S> extends GenericIndicator<S>

   This interface represents implementations of the Hypervolume quality indicator

   :author: Antonio J. Nebro , Juan J. Durillo

Constructors
------------
Hypervolume
^^^^^^^^^^^

.. java:constructor:: public Hypervolume()
   :outertype: Hypervolume

Hypervolume
^^^^^^^^^^^

.. java:constructor:: public Hypervolume(String referenceParetoFrontFile) throws FileNotFoundException
   :outertype: Hypervolume

Hypervolume
^^^^^^^^^^^

.. java:constructor:: public Hypervolume(Front referenceParetoFront)
   :outertype: Hypervolume

Methods
-------
computeHypervolumeContribution
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public abstract List<S> computeHypervolumeContribution(List<S> solutionList, List<S> referenceFrontList)
   :outertype: Hypervolume

getName
^^^^^^^

.. java:method:: @Override public String getName()
   :outertype: Hypervolume

getOffset
^^^^^^^^^

.. java:method:: public abstract double getOffset()
   :outertype: Hypervolume

isTheLowerTheIndicatorValueTheBetter
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public boolean isTheLowerTheIndicatorValueTheBetter()
   :outertype: Hypervolume

setOffset
^^^^^^^^^

.. java:method:: public abstract void setOffset(double offset)
   :outertype: Hypervolume

