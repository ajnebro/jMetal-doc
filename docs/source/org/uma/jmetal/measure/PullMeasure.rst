PullMeasure
===========

.. java:package:: org.uma.jmetal.measure
   :noindex:

.. java:type:: public interface PullMeasure<Value> extends Measure<Value>

   A \ :java:ref:`PullMeasure`\  is a \ :java:ref:`Measure`\  from which the \ :java:ref:`Value`\  can be accessed on demand through the \ :java:ref:`get()`\  method. As such, a \ :java:ref:`PullMeasure`\  should ensure that its current \ :java:ref:`Value`\  is always available or generated before to be returned by \ :java:ref:`get()`\ .

   :author: Created by Antonio J. Nebro on 21/10/14 based on the ideas of Matthieu Vergne
   :param <Value>: the type of value the \ :java:ref:`PullMeasure`\  can provide

Methods
-------
get
^^^

.. java:method:: public Value get()
   :outertype: PullMeasure

   :return: the current \ :java:ref:`Value`\  of the \ :java:ref:`Measure`\

