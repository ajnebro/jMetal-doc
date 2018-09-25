.. java:import:: java.io Serializable

Problem
=======

.. java:package:: org.uma.jmetal.problem
   :noindex:

.. java:type:: public interface Problem<S> extends Serializable

   Interface representing a multi-objective optimization problem

   :author: Antonio J. Nebro
   :param <S>: Encoding

Methods
-------
createSolution
^^^^^^^^^^^^^^

.. java:method::  S createSolution()
   :outertype: Problem

evaluate
^^^^^^^^

.. java:method::  void evaluate(S solution)
   :outertype: Problem

getName
^^^^^^^

.. java:method::  String getName()
   :outertype: Problem

getNumberOfConstraints
^^^^^^^^^^^^^^^^^^^^^^

.. java:method::  int getNumberOfConstraints()
   :outertype: Problem

getNumberOfObjectives
^^^^^^^^^^^^^^^^^^^^^

.. java:method::  int getNumberOfObjectives()
   :outertype: Problem

getNumberOfVariables
^^^^^^^^^^^^^^^^^^^^

.. java:method::  int getNumberOfVariables()
   :outertype: Problem

