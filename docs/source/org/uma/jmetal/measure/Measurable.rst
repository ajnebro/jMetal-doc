Measurable
==========

.. java:package:: org.uma.jmetal.measure
   :noindex:

.. java:type:: public interface Measurable

   A \ :java:ref:`Measurable`\  entity is an entity which provides one or several \ :java:ref:`Measure`\ s. To keep it simple, these \ :java:ref:`Measure`\ s are provided through a \ :java:ref:`MeasureManager`\ .

   :author: Created by Antonio J. Nebro on 21/10/14 based on the ideas of Matthieu Vergne

Methods
-------
getMeasureManager
^^^^^^^^^^^^^^^^^

.. java:method:: public MeasureManager getMeasureManager()
   :outertype: Measurable

   :return: the \ :java:ref:`MeasureManager`\  which stores all the \ :java:ref:`Measure`\ s supported by this \ :java:ref:`Measurable`\  entity

