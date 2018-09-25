.. java:import:: org.uma.jmetal.measure Measure

.. java:import:: org.uma.jmetal.measure MeasureListener

.. java:import:: org.uma.jmetal.measure PushMeasure

.. java:import:: java.util HashSet

.. java:import:: java.util Set

SimplePushMeasure
=================

.. java:package:: org.uma.jmetal.measure.impl
   :noindex:

.. java:type:: @SuppressWarnings public class SimplePushMeasure<Value> extends SimpleMeasure<Value> implements PushMeasure<Value>

   \ :java:ref:`SimplePushMeasure`\  is a basic implementation of \ :java:ref:`PushMeasure`\ . As a \ :java:ref:`PushMeasure`\ , it is intended to be fed by the algorithm while external entities should use \ :java:ref:`register(MeasureListener)`\  to be notified in real time. For the algorithm to feed it, it should provide a solution and its value to \ :java:ref:`push(Object,Object)`\ , leading to the notification of the registered observers.

   :author: Matthieu Vergne
   :param <Value>:

Constructors
------------
SimplePushMeasure
^^^^^^^^^^^^^^^^^

.. java:constructor:: public SimplePushMeasure(String name, String description)
   :outertype: SimplePushMeasure

   Create a \ :java:ref:`SimplePushMeasure`\  with a given name and a given description.

   :param name: the name of the \ :java:ref:`Measure`\
   :param description: the description of the \ :java:ref:`Measure`\

SimplePushMeasure
^^^^^^^^^^^^^^^^^

.. java:constructor:: public SimplePushMeasure(String name)
   :outertype: SimplePushMeasure

   Create a \ :java:ref:`SimplePushMeasure`\  with a given name and a \ ``null``\  description.

   :param name: the name of the \ :java:ref:`Measure`\

SimplePushMeasure
^^^^^^^^^^^^^^^^^

.. java:constructor:: public SimplePushMeasure()
   :outertype: SimplePushMeasure

   Create a \ :java:ref:`SimplePushMeasure`\  with the class name as its name and a \ ``null``\  description.

Methods
-------
push
^^^^

.. java:method:: public void push(Value value)
   :outertype: SimplePushMeasure

   Notify the observers which has registered a \ :java:ref:`MeasureListener`\  through \ :java:ref:`register(MeasureListener)`\  about a value.

   :param value: the value to send to the observers

register
^^^^^^^^

.. java:method:: @Override public void register(MeasureListener<Value> listener)
   :outertype: SimplePushMeasure

unregister
^^^^^^^^^^

.. java:method:: @Override public void unregister(MeasureListener<Value> listener)
   :outertype: SimplePushMeasure

