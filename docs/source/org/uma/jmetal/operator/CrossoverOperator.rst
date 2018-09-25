.. java:import:: java.util List

CrossoverOperator
=================

.. java:package:: org.uma.jmetal.operator
   :noindex:

.. java:type:: public interface CrossoverOperator<Source> extends Operator<List<Source>, List<Source>>

   Interface representing crossover operators. They will receive a list of solutions and return another list of solutions

   :author: Antonio J. Nebro
   :param <Source>: The class of the solutions

Methods
-------
getNumberOfGeneratedChildren
^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method::  int getNumberOfGeneratedChildren()
   :outertype: CrossoverOperator

getNumberOfRequiredParents
^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method::  int getNumberOfRequiredParents()
   :outertype: CrossoverOperator

