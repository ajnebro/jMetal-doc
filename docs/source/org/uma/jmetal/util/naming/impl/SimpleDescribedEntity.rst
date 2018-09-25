.. java:import:: org.uma.jmetal.util.naming DescribedEntity

SimpleDescribedEntity
=====================

.. java:package:: org.uma.jmetal.util.naming.impl
   :noindex:

.. java:type:: public class SimpleDescribedEntity implements DescribedEntity

   \ :java:ref:`SimpleDescribedEntity`\  is a basic implementation of \ :java:ref:`DescribedEntity`\ . It provides a basic support for the most generic properties required by this interface.

   :author: Matthieu Vergne

Constructors
------------
SimpleDescribedEntity
^^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public SimpleDescribedEntity(String name, String description)
   :outertype: SimpleDescribedEntity

   Create a \ :java:ref:`SimpleDescribedEntity`\  with a given name and a given description.

   :param name: the name of the \ :java:ref:`DescribedEntity`\
   :param description: the description of the \ :java:ref:`DescribedEntity`\

SimpleDescribedEntity
^^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public SimpleDescribedEntity(String name)
   :outertype: SimpleDescribedEntity

   Create a \ :java:ref:`SimpleDescribedEntity`\  with a given name and a \ ``null``\  description.

   :param name: the name of the \ :java:ref:`DescribedEntity`\

SimpleDescribedEntity
^^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public SimpleDescribedEntity()
   :outertype: SimpleDescribedEntity

   Create a \ :java:ref:`SimpleDescribedEntity`\  with the class name as its name and a \ ``null``\  description.

Methods
-------
getDescription
^^^^^^^^^^^^^^

.. java:method:: @Override public String getDescription()
   :outertype: SimpleDescribedEntity

getName
^^^^^^^

.. java:method:: @Override public String getName()
   :outertype: SimpleDescribedEntity

setDescription
^^^^^^^^^^^^^^

.. java:method:: public void setDescription(String description)
   :outertype: SimpleDescribedEntity

   :param description: the new description of this \ :java:ref:`DescribedEntity`\

setName
^^^^^^^

.. java:method:: public void setName(String name)
   :outertype: SimpleDescribedEntity

   :param name: the new name of this \ :java:ref:`DescribedEntity`\

toString
^^^^^^^^

.. java:method:: @Override public String toString()
   :outertype: SimpleDescribedEntity

