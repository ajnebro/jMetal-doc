.. java:import:: org.uma.jmetal.util.pseudorandom PseudoRandomGenerator

.. java:import:: java.util HashSet

.. java:import:: java.util Objects

.. java:import:: java.util Optional

.. java:import:: java.util Set

.. java:import:: java.util.function Consumer

AuditableRandomGenerator
========================

.. java:package:: org.uma.jmetal.util.pseudorandom.impl
   :noindex:

.. java:type:: @SuppressWarnings public class AuditableRandomGenerator implements PseudoRandomGenerator

   An \ :java:ref:`AuditableRandomGenerator`\  is a \ :java:ref:`PseudoRandomGenerator`\  which can be audited to know when a random generation method is called.

   :author: Matthieu Vergne

Constructors
------------
AuditableRandomGenerator
^^^^^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public AuditableRandomGenerator(PseudoRandomGenerator generator)
   :outertype: AuditableRandomGenerator

Methods
-------
addListener
^^^^^^^^^^^

.. java:method:: public void addListener(Consumer<Audit> listener)
   :outertype: AuditableRandomGenerator

getName
^^^^^^^

.. java:method:: @Override public String getName()
   :outertype: AuditableRandomGenerator

getSeed
^^^^^^^

.. java:method:: @Override public long getSeed()
   :outertype: AuditableRandomGenerator

nextDouble
^^^^^^^^^^

.. java:method:: @Override public double nextDouble(double lowerBound, double upperBound)
   :outertype: AuditableRandomGenerator

nextDouble
^^^^^^^^^^

.. java:method:: @Override public double nextDouble()
   :outertype: AuditableRandomGenerator

nextInt
^^^^^^^

.. java:method:: @Override public int nextInt(int lowerBound, int upperBound)
   :outertype: AuditableRandomGenerator

removeListener
^^^^^^^^^^^^^^

.. java:method:: public void removeListener(Consumer<Audit> listener)
   :outertype: AuditableRandomGenerator

setSeed
^^^^^^^

.. java:method:: @Override public void setSeed(long seed)
   :outertype: AuditableRandomGenerator

