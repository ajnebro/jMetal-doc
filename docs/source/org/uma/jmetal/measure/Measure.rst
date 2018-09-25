.. java:import:: org.uma.jmetal.algorithm Algorithm

.. java:import:: org.uma.jmetal.util.naming DescribedEntity

.. java:import:: java.io Serializable

Measure
=======

.. java:package:: org.uma.jmetal.measure
   :noindex:

.. java:type:: public interface Measure<Value> extends DescribedEntity, Serializable

   A \ :java:ref:`Measure`\  aims at providing the \ :java:ref:`Value`\  of a specific property, typically of an \ :java:ref:`Algorithm`\ . In order to facilitate external uses, it implements the methods of \ :java:ref:`DescribedEntity`\ .

   :author: Created by Antonio J. Nebro on 21/10/14 based on the ideas of Matthieu Vergne
   :param <Value>: the type of value the \ :java:ref:`Measure`\  can provide

