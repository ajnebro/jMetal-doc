.. java:import:: org.uma.jmetal.measure Measure

.. java:import:: org.uma.jmetal.measure MeasureListener

.. java:import:: org.uma.jmetal.measure PullMeasure

.. java:import:: org.uma.jmetal.measure PushMeasure

.. java:import:: org.uma.jmetal.util.naming DescribedEntity

.. java:import:: org.uma.jmetal.util.naming.impl SimpleDescribedEntity

PullPushMeasure
===============

.. java:package:: org.uma.jmetal.measure.impl
   :noindex:

.. java:type:: @SuppressWarnings public class PullPushMeasure<Value> implements PullMeasure<Value>, PushMeasure<Value>

   A \ :java:ref:`PullPushMeasure`\  aims at providing both the \ :java:ref:`PushMeasure`\  and \ :java:ref:`PullMeasure`\  abilities into a single \ :java:ref:`Measure`\ . One could simply build a brand new \ :java:ref:`Measure`\  by calling \ :java:ref:`PullPushMeasure(String,String)`\ , but in the case where some existing measures are available, he can wrap them into a \ :java:ref:`PullPushMeasure`\  by calling \ :java:ref:`PullPushMeasure(PushMeasure,Object)`\  or other constructors taking a \ :java:ref:`Measure`\  as argument.

   :author: Matthieu Vergne
   :param <Value>:

Constructors
------------
PullPushMeasure
^^^^^^^^^^^^^^^

.. java:constructor:: public PullPushMeasure(PullMeasure<Value> pull, PushMeasure<Value> push, DescribedEntity reference)
   :outertype: PullPushMeasure

   Create a \ :java:ref:`PullPushMeasure`\  which wraps both a \ :java:ref:`PullMeasure`\  and a \ :java:ref:`PushMeasure`\ . The assumption is that both \ :java:ref:`Measure`\ s already represent the same \ :java:ref:`Measure`\  (i.e. the same \ :java:ref:`Value`\ ) but were implemented separately. Instantiating a \ :java:ref:`PullPushMeasure`\  this way allows to merge them easily without creating a completely new measure. Don't use this constructor to merge two different \ :java:ref:`Measure`\ s. The last parameter is generally used to specify which of the two \ :java:ref:`Measure`\ s should be used for \ :java:ref:`getName()`\  and \ :java:ref:`getDescription()`\ , but you can also provide a completely new instance to change them.

   :param pull: the \ :java:ref:`PullMeasure`\  to wrap
   :param push: the \ :java:ref:`PushMeasure`\  to wrap
   :param reference: the reference to use for the name and the description of this \ :java:ref:`PullPushMeasure`\

PullPushMeasure
^^^^^^^^^^^^^^^

.. java:constructor:: public PullPushMeasure(PullMeasure<Value> pull, PushMeasure<Value> push, String name, String description)
   :outertype: PullPushMeasure

   Equivalent to \ :java:ref:`PullPushMeasure(PullMeasure,PushMeasure,DescribedEntity)`\  but the reference parameter is replaced by the specific name and description that you want to provide. This is a shortcut to the creation of the \ :java:ref:`DescribedEntity`\  instance followed by the call of the reference-based method.

   :param pull: the \ :java:ref:`PullMeasure`\  to wrap
   :param push: the \ :java:ref:`PushMeasure`\  to wrap
   :param name: the name of the \ :java:ref:`PullPushMeasure`\
   :param description: the description of the \ :java:ref:`PullPushMeasure`\

PullPushMeasure
^^^^^^^^^^^^^^^

.. java:constructor:: public PullPushMeasure(PushMeasure<Value> push, Value initialValue)
   :outertype: PullPushMeasure

   Create a \ :java:ref:`PullPushMeasure`\  which wraps a \ :java:ref:`PushMeasure`\ . The \ :java:ref:`PullMeasure`\  ability corresponds the storage of the \ :java:ref:`Value`\  pushed by the \ :java:ref:`PushMeasure`\  in order to retrieve it on demand through \ :java:ref:`PullMeasure.get()`\ . The name and the description of the \ :java:ref:`PullPushMeasure`\  are the ones provided by the wrapped \ :java:ref:`PushMeasure`\ .

   :param push: the \ :java:ref:`PushMeasure`\  to wraps
   :param initialValue: the \ :java:ref:`Value`\  to return before the next notification of the \ :java:ref:`PushMeasure`\

PullPushMeasure
^^^^^^^^^^^^^^^

.. java:constructor:: public PullPushMeasure(String name, String description)
   :outertype: PullPushMeasure

   Create a \ :java:ref:`PullPushMeasure`\  from scratch.

   :param name: the name of the \ :java:ref:`PullPushMeasure`\
   :param description: the description of the \ :java:ref:`PullPushMeasure`\

Methods
-------
get
^^^

.. java:method:: @Override public Value get()
   :outertype: PullPushMeasure

getDescription
^^^^^^^^^^^^^^

.. java:method:: @Override public String getDescription()
   :outertype: PullPushMeasure

getName
^^^^^^^

.. java:method:: @Override public String getName()
   :outertype: PullPushMeasure

register
^^^^^^^^

.. java:method:: @Override public void register(MeasureListener<Value> listener)
   :outertype: PullPushMeasure

unregister
^^^^^^^^^^

.. java:method:: @Override public void unregister(MeasureListener<Value> listener)
   :outertype: PullPushMeasure

