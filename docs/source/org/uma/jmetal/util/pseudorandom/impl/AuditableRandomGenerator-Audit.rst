.. java:import:: org.uma.jmetal.util.pseudorandom PseudoRandomGenerator

.. java:import:: java.util HashSet

.. java:import:: java.util Objects

.. java:import:: java.util Optional

.. java:import:: java.util Set

.. java:import:: java.util.function Consumer

AuditableRandomGenerator.Audit
==============================

.. java:package:: org.uma.jmetal.util.pseudorandom.impl
   :noindex:

.. java:type:: public static class Audit
   :outertype: AuditableRandomGenerator

Constructors
------------
Audit
^^^^^

.. java:constructor:: public Audit(RandomMethod method, Bounds bounds, Number result)
   :outertype: AuditableRandomGenerator.Audit

Methods
-------
getBounds
^^^^^^^^^

.. java:method:: public Optional<Bounds> getBounds()
   :outertype: AuditableRandomGenerator.Audit

getMethod
^^^^^^^^^

.. java:method:: public RandomMethod getMethod()
   :outertype: AuditableRandomGenerator.Audit

getResult
^^^^^^^^^

.. java:method:: public Number getResult()
   :outertype: AuditableRandomGenerator.Audit

