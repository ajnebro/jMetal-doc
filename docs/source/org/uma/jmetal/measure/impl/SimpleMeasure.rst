.. java:import:: org.uma.jmetal.measure Measure

.. java:import:: org.uma.jmetal.util.naming.impl SimpleDescribedEntity

SimpleMeasure
=============

.. java:package:: org.uma.jmetal.measure.impl
   :noindex:

.. java:type:: @SuppressWarnings public class SimpleMeasure<Value> extends SimpleDescribedEntity implements Measure<Value>

   \ :java:ref:`SimpleMeasure`\  is a basic implementation of \ :java:ref:`Measure`\ . It provides a basic support for the most generic properties required by this interface.

   :author: Matthieu Vergne
   :param <Value>:

Constructors
------------
SimpleMeasure
^^^^^^^^^^^^^

.. java:constructor:: public SimpleMeasure(String name, String description)
   :outertype: SimpleMeasure

   Create a \ :java:ref:`SimpleMeasure`\  with a given name and a given description.

   :param name: the name of the \ :java:ref:`Measure`\
   :param description: the description of the \ :java:ref:`Measure`\

SimpleMeasure
^^^^^^^^^^^^^

.. java:constructor:: public SimpleMeasure(String name)
   :outertype: SimpleMeasure

   Create a \ :java:ref:`SimpleMeasure`\  with a given name and a \ ``null``\  description.

   :param name: the name of the \ :java:ref:`Measure`\

SimpleMeasure
^^^^^^^^^^^^^

.. java:constructor:: public SimpleMeasure()
   :outertype: SimpleMeasure

   Create a \ :java:ref:`SimpleMeasure`\  with the class name as its name and a \ ``null``\  description.

