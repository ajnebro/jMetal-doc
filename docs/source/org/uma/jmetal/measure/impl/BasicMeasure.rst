.. java:import:: org.uma.jmetal.measure PullMeasure

.. java:import:: org.uma.jmetal.measure PushMeasure

BasicMeasure
============

.. java:package:: org.uma.jmetal.measure.impl
   :noindex:

.. java:type:: @SuppressWarnings public class BasicMeasure<T> extends SimplePushMeasure<T> implements PullMeasure<T>, PushMeasure<T>

   A \ :java:ref:`BasicMeasure`\  provides a simple way to define a measure that merely stores a single value

   :author: Antonio J. Nebro

Constructors
------------
BasicMeasure
^^^^^^^^^^^^

.. java:constructor:: public BasicMeasure()
   :outertype: BasicMeasure

   Create a \ :java:ref:`BasicMeasure`\

Methods
-------
get
^^^

.. java:method:: @Override public synchronized T get()
   :outertype: BasicMeasure

   :return: the current value

push
^^^^

.. java:method:: @Override public void push(T value)
   :outertype: BasicMeasure

set
^^^

.. java:method:: public synchronized void set(T value)
   :outertype: BasicMeasure

   :param value: The value to be stored

