.. java:import:: org.uma.jmetal.util.pseudorandom.impl JavaRandomGenerator

.. java:import:: java.io Serializable

JMetalRandom
============

.. java:package:: org.uma.jmetal.util.pseudorandom
   :noindex:

.. java:type:: @SuppressWarnings public class JMetalRandom implements Serializable

   :author: Antonio J. Nebro

Methods
-------
getGeneratorName
^^^^^^^^^^^^^^^^

.. java:method:: public String getGeneratorName()
   :outertype: JMetalRandom

getInstance
^^^^^^^^^^^

.. java:method:: public static JMetalRandom getInstance()
   :outertype: JMetalRandom

getRandomGenerator
^^^^^^^^^^^^^^^^^^

.. java:method:: public PseudoRandomGenerator getRandomGenerator()
   :outertype: JMetalRandom

getSeed
^^^^^^^

.. java:method:: public long getSeed()
   :outertype: JMetalRandom

nextDouble
^^^^^^^^^^

.. java:method:: public double nextDouble()
   :outertype: JMetalRandom

nextDouble
^^^^^^^^^^

.. java:method:: public double nextDouble(double lowerBound, double upperBound)
   :outertype: JMetalRandom

nextInt
^^^^^^^

.. java:method:: public int nextInt(int lowerBound, int upperBound)
   :outertype: JMetalRandom

setRandomGenerator
^^^^^^^^^^^^^^^^^^

.. java:method:: public void setRandomGenerator(PseudoRandomGenerator randomGenerator)
   :outertype: JMetalRandom

setSeed
^^^^^^^

.. java:method:: public void setSeed(long seed)
   :outertype: JMetalRandom

