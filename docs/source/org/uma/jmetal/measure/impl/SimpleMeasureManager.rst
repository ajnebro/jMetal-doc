.. java:import:: org.uma.jmetal.measure Measure

.. java:import:: org.uma.jmetal.measure MeasureManager

.. java:import:: org.uma.jmetal.measure PullMeasure

.. java:import:: org.uma.jmetal.measure PushMeasure

.. java:import:: java.util Collection

.. java:import:: java.util HashMap

.. java:import:: java.util HashSet

.. java:import:: java.util Map

.. java:import:: java.util Map.Entry

SimpleMeasureManager
====================

.. java:package:: org.uma.jmetal.measure.impl
   :noindex:

.. java:type:: public class SimpleMeasureManager implements MeasureManager

   This \ :java:ref:`SimpleMeasureManager`\  provides a basic implementation to manage a collection of \ :java:ref:`Measure`\ s. One can use the setXxxMeasure() methods to configure the \ :java:ref:`MeasureManager`\  with the finest granularity, or exploit the centralized \ :java:ref:`setMeasure(Object,Measure)`\  to register a \ :java:ref:`Measure`\  depending on the interfaces it implements, or even use the massive \ :java:ref:`setAllMeasures(Map)`\  to register a set of \ :java:ref:`Measure`\ s at once. The corresponding removeXxx methods are also available for each case. However, the only way to access a \ :java:ref:`Measure`\  is through the finest granularity with \ :java:ref:`getPullMeasure(Object)`\  and \ :java:ref:`getPushMeasure(Object)`\ .

   :author: Matthieu Vergne

Methods
-------
getMeasureKeys
^^^^^^^^^^^^^^

.. java:method:: @Override public Collection<Object> getMeasureKeys()
   :outertype: SimpleMeasureManager

   Provides the keys of all the \ :java:ref:`Measure`\ s which are supported by this \ :java:ref:`SimpleMeasureManager`\ . If a key is provided, then at least one version is available through \ :java:ref:`getPullMeasure(Object)`\  or \ :java:ref:`getPushMeasure(Object)`\ .

getPullMeasure
^^^^^^^^^^^^^^

.. java:method:: @SuppressWarnings @Override public <T> PullMeasure<T> getPullMeasure(Object key)
   :outertype: SimpleMeasureManager

getPushMeasure
^^^^^^^^^^^^^^

.. java:method:: @SuppressWarnings @Override public <T> PushMeasure<T> getPushMeasure(Object key)
   :outertype: SimpleMeasureManager

removeAllMeasures
^^^^^^^^^^^^^^^^^

.. java:method:: public void removeAllMeasures(Iterable<? extends Object> keys)
   :outertype: SimpleMeasureManager

   Massive equivalent to \ :java:ref:`removeMeasure(Object)`\ .

   :param keys: the keys of the \ :java:ref:`Measure`\ s to remove

removeMeasure
^^^^^^^^^^^^^

.. java:method:: public void removeMeasure(Object key)
   :outertype: SimpleMeasureManager

   This method removes an entire \ :java:ref:`Measure`\ , meaning that if both a \ :java:ref:`PullMeasure`\  and a \ :java:ref:`PushMeasure`\  are registered for this key, then both are removed.

   :param key: the key of the \ :java:ref:`Measure`\  to remove

removePullMeasure
^^^^^^^^^^^^^^^^^

.. java:method:: public void removePullMeasure(Object key)
   :outertype: SimpleMeasureManager

   :param key: the key of the \ :java:ref:`PullMeasure`\  to remove

removePushMeasure
^^^^^^^^^^^^^^^^^

.. java:method:: public void removePushMeasure(Object key)
   :outertype: SimpleMeasureManager

   :param key: the key of the \ :java:ref:`PushMeasure`\  to remove

setAllMeasures
^^^^^^^^^^^^^^

.. java:method:: public void setAllMeasures(Map<? extends Object, ? extends Measure<?>> measures)
   :outertype: SimpleMeasureManager

   Massive equivalent of \ :java:ref:`setMeasure(Object,Measure)`\ .

   :param measures: the \ :java:ref:`Measure`\ s to register with their corresponding keys

setMeasure
^^^^^^^^^^

.. java:method:: public void setMeasure(Object key, Measure<?> measure)
   :outertype: SimpleMeasureManager

   This method call \ :java:ref:`setPullMeasure(Object,PullMeasure)`\  or \ :java:ref:`setPushMeasure(Object,PushMeasure)`\  depending on the interfaces implemented by the \ :java:ref:`Measure`\  given in argument. If both interfaces are implemented, both methods are called, allowing to register all the aspects of the \ :java:ref:`Measure`\  in one call.

   :param key: the key of the \ :java:ref:`Measure`\
   :param measure: the \ :java:ref:`Measure`\  to register

setPullMeasure
^^^^^^^^^^^^^^

.. java:method:: public void setPullMeasure(Object key, PullMeasure<?> measure)
   :outertype: SimpleMeasureManager

   :param key: the key of the \ :java:ref:`Measure`\
   :param measure: the \ :java:ref:`PullMeasure`\  to register

setPushMeasure
^^^^^^^^^^^^^^

.. java:method:: public void setPushMeasure(Object key, PushMeasure<?> measure)
   :outertype: SimpleMeasureManager

   :param key: the key of the \ :java:ref:`Measure`\
   :param measure: the \ :java:ref:`PushMeasure`\  to register

