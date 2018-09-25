.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util.solutionattribute SolutionAttribute

GenericSolutionAttribute
========================

.. java:package:: org.uma.jmetal.util.solutionattribute.impl
   :noindex:

.. java:type:: @SuppressWarnings public class GenericSolutionAttribute<S extends Solution<?>, V> implements SolutionAttribute<S, V>

   Generic class for implementing \ :java:ref:`SolutionAttribute`\  classes. By default, the identifier of a \ :java:ref:`SolutionAttribute`\  is the class object, but it can be set to a different value when constructing an instance.

   :author: Antonio J. Nebro

Constructors
------------
GenericSolutionAttribute
^^^^^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public GenericSolutionAttribute()
   :outertype: GenericSolutionAttribute

   Constructor

GenericSolutionAttribute
^^^^^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public GenericSolutionAttribute(Object id)
   :outertype: GenericSolutionAttribute

   Constructor

   :param id: Attribute identifier

Methods
-------
getAttribute
^^^^^^^^^^^^

.. java:method:: @SuppressWarnings @Override public V getAttribute(S solution)
   :outertype: GenericSolutionAttribute

getAttributeIdentifier
^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public Object getAttributeIdentifier()
   :outertype: GenericSolutionAttribute

setAttribute
^^^^^^^^^^^^

.. java:method:: @Override public void setAttribute(S solution, V value)
   :outertype: GenericSolutionAttribute

