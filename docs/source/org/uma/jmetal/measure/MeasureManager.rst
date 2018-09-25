.. java:import:: java.util Collection

MeasureManager
==============

.. java:package:: org.uma.jmetal.measure
   :noindex:

.. java:type:: public interface MeasureManager

   A \ :java:ref:`MeasureManager`\  aims at managing a set of \ :java:ref:`Measure`\ s. Typically, a \ :java:ref:`Measurable`\  entity would create a single \ :java:ref:`MeasureManager`\  to store all the \ :java:ref:`Measure`\ s it would like to support, each of them being identified by a key.  Because a \ :java:ref:`Measure`\  can be whether a \ :java:ref:`PullMeasure`\  or a \ :java:ref:`PushMeasure`\ , the two methods \ :java:ref:`getPullMeasure(Object)`\  and \ :java:ref:`getPushMeasure(Object)`\  are provided. It could be that a single \ :java:ref:`Measure`\  is also available through both (via a single instance implementing both interfaces or two different instances implementing each interface), leading to have both methods returning a non-\ ``null``\  value for the same key.

   :author: Created by Antonio J. Nebro on 21/10/14 based on the ideas of Matthieu Vergne

Methods
-------
getMeasureKeys
^^^^^^^^^^^^^^

.. java:method:: public Collection<Object> getMeasureKeys()
   :outertype: MeasureManager

   This method should return all the keys identifying the \ :java:ref:`Measure`\ s managed by this \ :java:ref:`MeasureManager`\ . More precisely, if \ :java:ref:`getPullMeasure(Object)`\  or \ :java:ref:`getPushMeasure(Object)`\  returns a non-\ ``null``\  value for a given key, then this key should be returned by \ :java:ref:`getMeasureKeys()`\ . However, it is not because a key is returned by \ :java:ref:`getMeasureKeys()`\  that it necessarily has a \ :java:ref:`PullMeasure`\  or a \ :java:ref:`PushMeasure`\  returned by this \ :java:ref:`MeasureManager`\ .

   :return: the set of keys identifying the managed \ :java:ref:`Measure`\ s

getPullMeasure
^^^^^^^^^^^^^^

.. java:method:: public <T> PullMeasure<T> getPullMeasure(Object key)
   :outertype: MeasureManager

   :param key: the key of the \ :java:ref:`Measure`\
   :return: the \ :java:ref:`PullMeasure`\  identified by this key

getPushMeasure
^^^^^^^^^^^^^^

.. java:method:: public <T> PushMeasure<T> getPushMeasure(Object key)
   :outertype: MeasureManager

   :param key: the key of the \ :java:ref:`Measure`\
   :return: the \ :java:ref:`PushMeasure`\  identified by this key

