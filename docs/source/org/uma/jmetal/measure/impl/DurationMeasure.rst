DurationMeasure
===============

.. java:package:: org.uma.jmetal.measure.impl
   :noindex:

.. java:type:: @SuppressWarnings public class DurationMeasure extends SimplePullMeasure<Long>

   This measure allows to have a simple way to compute the time spent in doing something. For instance, an algorithm can compute the time spent to run. In such a case, the algorithm would call \ :java:ref:`start()`\  at the beginning of the running and \ :java:ref:`stop()`\  at the end. Additional calls to these two methods can also be made during the running to exclude specific parts from the counting. At any time during (and after) the running, the \ :java:ref:`get()`\  method can be used to know how much time have been spent so far. If the algorithm is rerun, it will restart and the additional time will sum up to the time already spent before, but it can be avoided by resetting the measure with \ :java:ref:`reset()`\ .

   :author: Matthieu Vergne

Constructors
------------
DurationMeasure
^^^^^^^^^^^^^^^

.. java:constructor:: public DurationMeasure()
   :outertype: DurationMeasure

Methods
-------
get
^^^

.. java:method:: @Override public Long get()
   :outertype: DurationMeasure

   :return: the total time spent so far

reset
^^^^^

.. java:method:: public void reset()
   :outertype: DurationMeasure

   Reset the total time to zero. If a round is currently running, it is restarted.

start
^^^^^

.. java:method:: public void start()
   :outertype: DurationMeasure

   Start a round. If the round is already started, it has no effect.

stop
^^^^

.. java:method:: public void stop()
   :outertype: DurationMeasure

   Stop a round. If the round is already stopped, it has no effect.

