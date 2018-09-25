.. java:import:: org.uma.jmetal.util.naming DescribedEntity

.. java:import:: java.io Serializable

Algorithm
=========

.. java:package:: org.uma.jmetal.algorithm
   :noindex:

.. java:type:: public interface Algorithm<Result> extends Runnable, Serializable, DescribedEntity

   Interface representing an algorithm

   :author: Antonio J. Nebro
   :param <Result>: Result

Methods
-------
getResult
^^^^^^^^^

.. java:method::  Result getResult()
   :outertype: Algorithm

run
^^^

.. java:method::  void run()
   :outertype: Algorithm

