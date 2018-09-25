.. java:import:: org.uma.jmetal.util.pseudorandom PseudoRandomGenerator

.. java:import:: java.util Random

JavaRandomGenerator
===================

.. java:package:: org.uma.jmetal.util.pseudorandom.impl
   :noindex:

.. java:type:: @SuppressWarnings public class JavaRandomGenerator implements PseudoRandomGenerator

   :author: Antonio J. Nebro

Constructors
------------
JavaRandomGenerator
^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public JavaRandomGenerator()
   :outertype: JavaRandomGenerator

   Constructor

JavaRandomGenerator
^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public JavaRandomGenerator(long seed)
   :outertype: JavaRandomGenerator

   Constructor

Methods
-------
getName
^^^^^^^

.. java:method:: @Override public String getName()
   :outertype: JavaRandomGenerator

getSeed
^^^^^^^

.. java:method:: @Override public long getSeed()
   :outertype: JavaRandomGenerator

nextDouble
^^^^^^^^^^

.. java:method:: @Override public double nextDouble(double lowerBound, double upperBound)
   :outertype: JavaRandomGenerator

nextDouble
^^^^^^^^^^

.. java:method:: @Override public double nextDouble()
   :outertype: JavaRandomGenerator

nextInt
^^^^^^^

.. java:method:: @Override public int nextInt(int lowerBound, int upperBound)
   :outertype: JavaRandomGenerator

setSeed
^^^^^^^

.. java:method:: @Override public void setSeed(long seed)
   :outertype: JavaRandomGenerator

