PushMeasure
===========

.. java:package:: org.uma.jmetal.measure
   :noindex:

.. java:type:: public interface PushMeasure<Value> extends Measure<Value>

   A \ :java:ref:`PushMeasure`\  is a \ :java:ref:`Measure`\  which provides its \ :java:ref:`Value`\  through notifications. As such, any observer on a \ :java:ref:`PushMeasure`\  should register a \ :java:ref:`MeasureListener`\  through \ :java:ref:`register(MeasureListener)`\  to specify what to do with the \ :java:ref:`Value`\  once it is received.

   :author: Created by Antonio J. Nebro on 21/10/14 based on the ideas of Matthieu Vergne
   :param <Value>: the type of value the \ :java:ref:`PushMeasure`\  can provide

Methods
-------
register
^^^^^^^^

.. java:method:: public void register(MeasureListener<Value> listener)
   :outertype: PushMeasure

   Register a \ :java:ref:`MeasureListener`\  to use the \ :java:ref:`Value`\ s of the \ :java:ref:`PushMeasure`\  when they are generated.

   :param listener: the \ :java:ref:`MeasureListener`\  to register

unregister
^^^^^^^^^^

.. java:method:: public void unregister(MeasureListener<Value> listener)
   :outertype: PushMeasure

   Unregister a \ :java:ref:`MeasureListener`\  registered with \ :java:ref:`register(MeasureListener)`\  to stop receiving the notifications of the \ :java:ref:`PushMeasure`\ .

   :param listener: the \ :java:ref:`MeasureListener`\  to unregister

