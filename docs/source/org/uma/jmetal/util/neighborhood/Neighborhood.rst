.. java:import:: java.io Serializable

.. java:import:: java.util List

Neighborhood
============

.. java:package:: org.uma.jmetal.util.neighborhood
   :noindex:

.. java:type:: public interface Neighborhood<S> extends Serializable

   Interface representing a neighborhood of a given solution in a list of solutions

   :author: Antonio J. Nebro

Methods
-------
getNeighbors
^^^^^^^^^^^^

.. java:method:: public List<S> getNeighbors(List<S> solutionList, int solutionIndex)
   :outertype: Neighborhood

