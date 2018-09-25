.. java:import:: org.uma.jmetal.measure MeasureListener

.. java:import:: org.uma.jmetal.measure PullMeasure

.. java:import:: org.uma.jmetal.measure PushMeasure

.. java:import:: java.util Collection

.. java:import:: java.util LinkedList

.. java:import:: java.util Map

.. java:import:: java.util WeakHashMap

CountingMeasure
===============

.. java:package:: org.uma.jmetal.measure.impl
   :noindex:

.. java:type:: @SuppressWarnings public class CountingMeasure extends SimplePushMeasure<Long> implements PullMeasure<Long>, PushMeasure<Long>

   A \ :java:ref:`CountingMeasure`\  provides a simple way to evaluate a number of occurrences. For instance, it can be used to count how many solutions have been generated within an algorithm, how many evaluations have been computed, how many rounds have been run, etc. If these occurrences are provided by some \ :java:ref:`PushMeasure`\ s, you can use \ :java:ref:`link(PushMeasure)`\  to register the \ :java:ref:`CountingMeasure`\  to these \ :java:ref:`PushMeasure`\ s. Otherwise, use \ :java:ref:`increment()`\  when the \ :java:ref:`CountingMeasure`\  need to count one more occurrence. In order to get the count, one can access it immediately through \ :java:ref:`get()`\  or when it is updated by registering a listener with \ :java:ref:`register(MeasureListener)`\ .

   :author: Matthieu Vergne

Fields
------
count
^^^^^

.. java:field::  long count
   :outertype: CountingMeasure

   The current amount of occurrences counted.

Constructors
------------
CountingMeasure
^^^^^^^^^^^^^^^

.. java:constructor:: public CountingMeasure(String name, String description, long initialCount)
   :outertype: CountingMeasure

   Create a \ :java:ref:`CountingMeasure`\  which starts at a given value. The next value to be pushed to the registered observers will be this value + 1.

   :param name: the name of the measure
   :param description: the description of the measure
   :param initialCount: the value to start from

CountingMeasure
^^^^^^^^^^^^^^^

.. java:constructor:: public CountingMeasure(String name, String description)
   :outertype: CountingMeasure

   Create a \ :java:ref:`CountingMeasure`\  starting from zero. The registered observers will receive their first notification when it will increment to 1.

   :param name: the name of the measure
   :param description: the description of the measure

CountingMeasure
^^^^^^^^^^^^^^^

.. java:constructor:: public CountingMeasure(long initialCount)
   :outertype: CountingMeasure

   Create a \ :java:ref:`CountingMeasure`\  which starts at a given value. The next value to be pushed to the registered observers will be this value + 1. A default name and description are used.

   :param initialCount: the value to start from

CountingMeasure
^^^^^^^^^^^^^^^

.. java:constructor:: public CountingMeasure()
   :outertype: CountingMeasure

   Create a \ :java:ref:`CountingMeasure`\  starting from zero. The registered observers will receive their first notification when it will increment to 1. A default name and description are used.

Methods
-------
finalize
^^^^^^^^

.. java:method:: @Override protected void finalize() throws Throwable
   :outertype: CountingMeasure

get
^^^

.. java:method:: @Override public synchronized Long get()
   :outertype: CountingMeasure

   :return: the current amount of occurrences counted

increment
^^^^^^^^^

.. java:method:: public synchronized void increment()
   :outertype: CountingMeasure

   Add 1 to the current count and push its value to all the registered observers.

increment
^^^^^^^^^

.. java:method:: public synchronized void increment(long amount)
   :outertype: CountingMeasure

   Increment the current count in a given amount. If the amount is zero, no change occurs, thus no notification is sent.

   :param amount: the amount to add

link
^^^^

.. java:method:: public <T> void link(PushMeasure<T> measure)
   :outertype: CountingMeasure

   If this \ :java:ref:`CountingMeasure`\  is used to count the number of time a \ :java:ref:`PushMeasure`\  notifies its observers, you can use this method to link them. The \ :java:ref:`CountingMeasure`\  will automatically register a \ :java:ref:`MeasureListener`\  on the \ :java:ref:`PushMeasure`\  such that, every time the \ :java:ref:`PushMeasure`\  send a notification, \ :java:ref:`CountingMeasure.increment()`\  is called. You can link several \ :java:ref:`PushMeasure`\ s at the same time, but each of their notifications will increment the counter, leading to summing their notifications. When a \ :java:ref:`PushMeasure`\  should not be considered anymore, use \ :java:ref:`unlink(PushMeasure)`\  to remove the link.

   :param measure: the \ :java:ref:`PushMeasure`\  to link

reset
^^^^^

.. java:method:: public synchronized void reset()
   :outertype: CountingMeasure

   Restart the counter to zero. Generate a notification if the value was not zero.

reset
^^^^^

.. java:method:: public synchronized void reset(long value)
   :outertype: CountingMeasure

   Restart the counter to a given value. Generate a notification if the value was different.

   :param value: the value to restart from

unlink
^^^^^^

.. java:method:: @SuppressWarnings public <T> void unlink(PushMeasure<T> measure)
   :outertype: CountingMeasure

   If you have linked a \ :java:ref:`PushMeasure`\  through \ :java:ref:`link(PushMeasure)`\ , you can discard the link by using this method.

   :param measure: the \ :java:ref:`PushMeasure`\  to unlink

