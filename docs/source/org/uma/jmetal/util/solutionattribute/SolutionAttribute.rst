.. java:import:: java.io Serializable

SolutionAttribute
=================

.. java:package:: org.uma.jmetal.util.solutionattribute
   :noindex:

.. java:type:: public interface SolutionAttribute<S, V> extends Serializable

   Attributes allows to extend the solution classes to incorporate data required by operators or algorithms manipulating them.

   :author: Antonio J. Nebro

Methods
-------
getAttribute
^^^^^^^^^^^^

.. java:method:: public V getAttribute(S solution)
   :outertype: SolutionAttribute

getAttributeIdentifier
^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public Object getAttributeIdentifier()
   :outertype: SolutionAttribute

setAttribute
^^^^^^^^^^^^

.. java:method:: public void setAttribute(S solution, V value)
   :outertype: SolutionAttribute

