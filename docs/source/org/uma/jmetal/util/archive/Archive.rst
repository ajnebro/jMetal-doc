.. java:import:: java.io Serializable

.. java:import:: java.util List

Archive
=======

.. java:package:: org.uma.jmetal.util.archive
   :noindex:

.. java:type:: public interface Archive<S> extends Serializable

   Interface representing an archive of solutions

   :author: Antonio J. Nebro

Methods
-------
add
^^^

.. java:method::  boolean add(S solution)
   :outertype: Archive

get
^^^

.. java:method::  S get(int index)
   :outertype: Archive

getSolutionList
^^^^^^^^^^^^^^^

.. java:method::  List<S> getSolutionList()
   :outertype: Archive

size
^^^^

.. java:method::  int size()
   :outertype: Archive

