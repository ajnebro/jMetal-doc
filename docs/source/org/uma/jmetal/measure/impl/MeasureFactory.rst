.. java:import:: org.uma.jmetal.measure Measure

.. java:import:: org.uma.jmetal.measure MeasureListener

.. java:import:: org.uma.jmetal.measure PullMeasure

.. java:import:: org.uma.jmetal.measure PushMeasure

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: java.lang.ref WeakReference

.. java:import:: java.lang.reflect Field

.. java:import:: java.lang.reflect InvocationTargetException

.. java:import:: java.lang.reflect Method

.. java:import:: java.util HashMap

.. java:import:: java.util Map

.. java:import:: java.util.logging Logger

MeasureFactory
==============

.. java:package:: org.uma.jmetal.measure.impl
   :noindex:

.. java:type:: public class MeasureFactory

   The \ :java:ref:`MeasureFactory`\  provides some useful methods to build specific \ :java:ref:`Measure`\ s.

   :author: Matthieu Vergne

Methods
-------
createPullFromPush
^^^^^^^^^^^^^^^^^^

.. java:method:: @SuppressWarnings public <Value> PullMeasure<Value> createPullFromPush(PushMeasure<Value> push, Value initialValue)
   :outertype: MeasureFactory

   Create a \ :java:ref:`PullMeasure`\  to backup the last \ :java:ref:`Value`\  of a \ :java:ref:`PushMeasure`\ . When the \ :java:ref:`PushMeasure`\  send a notification with a given \ :java:ref:`Value`\ , this \ :java:ref:`Value`\  is stored into a variable so that it can be retrieved at any time through the method \ :java:ref:`PullMeasure.get()`\ .

   :param push: a \ :java:ref:`PushMeasure`\  to backup
   :param initialValue: the \ :java:ref:`Value`\  to return before the next notification of the \ :java:ref:`PushMeasure`\  is sent
   :return: a \ :java:ref:`PullMeasure`\  allowing to retrieve the last value sent by the \ :java:ref:`PushMeasure`\ , or the initial value if it did not send any

createPullsFromFields
^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @SuppressWarnings public Map<String, PullMeasure<?>> createPullsFromFields(Object object)
   :outertype: MeasureFactory

   Create \ :java:ref:`PullMeasure`\ s based on the fields available from an instance, whatever it is. The \ :java:ref:`Class`\  of the instance is analyzed to retrieve its public fields and a \ :java:ref:`PullMeasure`\  is built for each of them. The name of the field is further exploited to identify the measure, such that the map returned use the name of the field as a key which maps to the \ :java:ref:`PullMeasure`\  built from this field. The \ :java:ref:`PullMeasure`\  itself is named by using the name of the field.

   :param object: the \ :java:ref:`Object`\  to cover
   :return: the \ :java:ref:`Map`\  which contains the names of the getter methods and the corresponding \ :java:ref:`PullMeasure`\  built from them

createPullsFromGetters
^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @SuppressWarnings public Map<String, PullMeasure<?>> createPullsFromGetters(Object object)
   :outertype: MeasureFactory

   Create \ :java:ref:`PullMeasure`\ s based on the getters available from an instance, whatever it is. The \ :java:ref:`Class`\  of the instance is analyzed to retrieve its public methods and a \ :java:ref:`PullMeasure`\  is built for each method which use a getter-like signature. The name of the method is further exploited to identify the measure, such that the map returned use the name of the method (without "get") as a key which maps to the \ :java:ref:`PullMeasure`\  built from this method. The \ :java:ref:`PullMeasure`\  itself is named by using the name of the method.

   :param object: the \ :java:ref:`Object`\  to cover
   :return: the \ :java:ref:`Map`\  which contains the names of the getter methods and the corresponding \ :java:ref:`PullMeasure`\  built from them

createPushFromPull
^^^^^^^^^^^^^^^^^^

.. java:method:: public <Value> PushMeasure<Value> createPushFromPull(PullMeasure<Value> pull, long period)
   :outertype: MeasureFactory

   Create a \ :java:ref:`PushMeasure`\  which checks at regular intervals the value of a \ :java:ref:`PullMeasure`\ . If the value have changed since the last check (or since the creation of the \ :java:ref:`PushMeasure`\ ), a notification will be generated by the \ :java:ref:`PushMeasure`\  with the new \ :java:ref:`Value`\ .  Notice that if the period is two small, the checking process could have a significant impact on performances, because a \ :java:ref:`Thread`\  is run in parallel to check regularly the \ :java:ref:`Value`\  modifications. If the period is too big, you could miss relevant notifications, especially if the \ :java:ref:`PullMeasure`\  change to a new \ :java:ref:`Value`\  and change back to its previous \ :java:ref:`Value`\  between two consecutive checks. In such a case, no notification will be sent because the \ :java:ref:`Value`\  during the two checks is equal.

   :param pull: the \ :java:ref:`PullMeasure`\  to cover
   :param period: the number of milliseconds between each check
   :return: a \ :java:ref:`PushMeasure`\  which will notify any change occurred on the \ :java:ref:`PullMeasure`\  at the given frequency

