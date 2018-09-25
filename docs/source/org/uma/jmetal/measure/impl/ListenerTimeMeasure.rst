.. java:import:: org.uma.jmetal.measure MeasureListener

.. java:import:: org.uma.jmetal.measure MeasureManager

.. java:import:: org.uma.jmetal.measure PullMeasure

.. java:import:: org.uma.jmetal.measure PushMeasure

.. java:import:: java.util Collection

.. java:import:: java.util LinkedList

.. java:import:: java.util WeakHashMap

ListenerTimeMeasure
===================

.. java:package:: org.uma.jmetal.measure.impl
   :noindex:

.. java:type:: @SuppressWarnings public class ListenerTimeMeasure extends SimplePullMeasure<Long> implements PullMeasure<Long>

   This measure is a facility to evaluate the time spent in \ :java:ref:`MeasureListener`\ s registered in \ :java:ref:`PushMeasure`\ s. In order to measure the time spent in a \ :java:ref:`MeasureListener`\ , you should wrap it by calling \ :java:ref:`wrapListener(MeasureListener)`\ . The wrapper returned should be used instead of the original \ :java:ref:`MeasureListener`\  to allow the \ :java:ref:`ListenerTimeMeasure`\  to account for its execution time. If you want to wrap automatically all the \ :java:ref:`MeasureListener`\ s registered to a given \ :java:ref:`PushMeasure`\ , you can wrap the \ :java:ref:`PushMeasure`\  through \ :java:ref:`wrapMeasure(PushMeasure)`\ : all the \ :java:ref:`MeasureListener`\ s registered to the wrapper will be wrapped too. You can restart the evaluation by calling \ :java:ref:`reset()`\ .  Notice that the time accounted is not the physical time but the processing time: if several listeners run in parallel, their execution time is summed as if they were running sequentially, thus you can have a measured time which is superior to the physical time spent. If you want to measure the physical time spent in the execution of parallel runs, you should use another way.

   :author: Matthieu Vergne

Methods
-------
get
^^^

.. java:method:: @Override public Long get()
   :outertype: ListenerTimeMeasure

   :return: the time spent in the wrapped \ :java:ref:`MeasureListener`\ s

reset
^^^^^

.. java:method:: public void reset()
   :outertype: ListenerTimeMeasure

   This method reset the time measured to zero. Notice that \ :java:ref:`MeasureListener`\ s which are still running will be affected consequently: their execution time will be measured from the reset time, not from their own starting time.

wrapListener
^^^^^^^^^^^^

.. java:method:: public <Value> MeasureListener<Value> wrapListener(MeasureListener<Value> wrapped)
   :outertype: ListenerTimeMeasure

   This method wrap a \ :java:ref:`MeasureListener`\  (the wrapped) into another one (the wrapper). Any notification made via the wrapper will allow to measure how much time has been spent by the wrapped to treat this notification.  The wrapped listener is not changed, thus it can be reused in other \ :java:ref:`PushMeasure`\ s that we don't want to consider. If a wrapper has already been made for the given wrapped, it will be returned and no new one will be instantiated (weak references are used to not keep in memory the unused wrappers).

   :param wrapped: the \ :java:ref:`MeasureListener`\  to wrap
   :return: the \ :java:ref:`MeasureListener`\  wrapper

wrapManager
^^^^^^^^^^^

.. java:method:: public <Value> MeasureManager wrapManager(MeasureManager wrapped, Object measureKey)
   :outertype: ListenerTimeMeasure

   This method wrap a \ :java:ref:`MeasureManager`\  (the wrapped) into another one (the wrapper) which provides the same measures, excepted that any \ :java:ref:`PushMeasure`\  returned by the wrapper will be automatically wrapped via \ :java:ref:`wrapMeasure(PushMeasure)`\ . This allows to ensure that any \ :java:ref:`MeasureListener`\  registered to the \ :java:ref:`PushMeasure`\ s provided by the wrapper will be considered, independently of who registers it or when it is registered. You can also provide an additional key to add this \ :java:ref:`ListenerTimeMeasure`\  to the wrapper.  The wrapped manager is not changed, thus it can be reused to register \ :java:ref:`MeasureListener`\ s that we don't want to consider.

   :param wrapped: the \ :java:ref:`MeasureManager`\  to wrap
   :param measureKey: the key that the wrapper should use for this \ :java:ref:`ListenerTimeMeasure`\ , \ ``null``\  if it should not use it
   :return: the \ :java:ref:`MeasureManager`\  wrapper

wrapMeasure
^^^^^^^^^^^

.. java:method:: public <Value> PushMeasure<Value> wrapMeasure(PushMeasure<Value> wrapped)
   :outertype: ListenerTimeMeasure

   This method wrap a \ :java:ref:`PushMeasure`\  (the wrapped) into another one (the wrapper). Any \ :java:ref:`MeasureListener`\  registered to the wrapper will be automatically wrapped via \ :java:ref:`wrapListener(MeasureListener)`\ . This allows to ensure that any \ :java:ref:`MeasureListener`\  registered will be considered, independently of who registers it or when it is registered.  The wrapped measure is not changed, thus it can be reused to register \ :java:ref:`MeasureListener`\ s that we don't want to consider. If a wrapper has already been made for the given wrapped, it will be returned and no new one will be instantiated (weak references are used to not keep in memory the unused wrappers).

   :param wrapped: the \ :java:ref:`PushMeasure`\  to wrap
   :return: the \ :java:ref:`PushMeasure`\  wrapper

