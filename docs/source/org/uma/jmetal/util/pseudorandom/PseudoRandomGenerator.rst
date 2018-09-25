.. java:import:: java.io Serializable

PseudoRandomGenerator
=====================

.. java:package:: org.uma.jmetal.util.pseudorandom
   :noindex:

.. java:type:: public interface PseudoRandomGenerator extends Serializable

   :author: Antonio J. Nebro

Methods
-------
getName
^^^^^^^

.. java:method:: public String getName()
   :outertype: PseudoRandomGenerator

getSeed
^^^^^^^

.. java:method:: public long getSeed()
   :outertype: PseudoRandomGenerator

nextDouble
^^^^^^^^^^

.. java:method:: public double nextDouble(double lowerBound, double upperBound)
   :outertype: PseudoRandomGenerator

nextDouble
^^^^^^^^^^

.. java:method:: public double nextDouble()
   :outertype: PseudoRandomGenerator

nextInt
^^^^^^^

.. java:method:: public int nextInt(int lowerBound, int upperBound)
   :outertype: PseudoRandomGenerator

setSeed
^^^^^^^

.. java:method:: public void setSeed(long seed)
   :outertype: PseudoRandomGenerator

