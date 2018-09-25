.. java:import:: org.uma.jmetal.measure Measure

.. java:import:: org.uma.jmetal.measure PullMeasure

SimplePullMeasure
=================

.. java:package:: org.uma.jmetal.measure.impl
   :noindex:

.. java:type:: @SuppressWarnings public abstract class SimplePullMeasure<Value> extends SimpleMeasure<Value> implements PullMeasure<Value>

   \ :java:ref:`SimplePullMeasure`\  is a basic implementation of \ :java:ref:`PullMeasure`\ . As a \ :java:ref:`PullMeasure`\ , it is intended to be used by external entities through its \ :java:ref:`get()`\  method. This method must be implemented by the algorithm to specify how the value can be retrieved.

   :author: Matthieu Vergne
   :param <Value>:

Constructors
------------
SimplePullMeasure
^^^^^^^^^^^^^^^^^

.. java:constructor:: public SimplePullMeasure(String name, String description)
   :outertype: SimplePullMeasure

   Create a \ :java:ref:`SimplePullMeasure`\  with a given name and a given description.

   :param name: the name of the \ :java:ref:`Measure`\
   :param description: the description of the \ :java:ref:`Measure`\

SimplePullMeasure
^^^^^^^^^^^^^^^^^

.. java:constructor:: public SimplePullMeasure(String name)
   :outertype: SimplePullMeasure

   Create a \ :java:ref:`SimplePullMeasure`\  with a given name and a \ ``null``\  description.

   :param name: the name of the \ :java:ref:`Measure`\

SimplePullMeasure
^^^^^^^^^^^^^^^^^

.. java:constructor:: public SimplePullMeasure()
   :outertype: SimplePullMeasure

   Create a \ :java:ref:`SimplePullMeasure`\  with the class name as its name and a \ ``null``\  description.

