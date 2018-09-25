.. java:import:: java.io Serializable

Operator
========

.. java:package:: org.uma.jmetal.operator
   :noindex:

.. java:type:: public interface Operator<Source, Result> extends Serializable

   Interface representing an operator

   :author: Antonio J. Nebro
   :param <Source>: Source Class of the object to be operated with
   :param <Result>: Result Class of the result obtained after applying the operator

Methods
-------
execute
^^^^^^^

.. java:method::  Result execute(Source source)
   :outertype: Operator

   :param source: The data to process

