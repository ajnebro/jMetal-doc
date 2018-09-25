.. java:import:: org.apache.commons.math3.random MersenneTwister

.. java:import:: org.uma.jmetal.util.pseudorandom PseudoRandomGenerator

MersenneTwisterGenerator
========================

.. java:package:: org.uma.jmetal.util.pseudorandom.impl
   :noindex:

.. java:type:: @SuppressWarnings public class MersenneTwisterGenerator implements PseudoRandomGenerator

   :author: Antonio J. Nebro

Constructors
------------
MersenneTwisterGenerator
^^^^^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public MersenneTwisterGenerator()
   :outertype: MersenneTwisterGenerator

   Constructor

MersenneTwisterGenerator
^^^^^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public MersenneTwisterGenerator(long seed)
   :outertype: MersenneTwisterGenerator

   Constructor

Methods
-------
getName
^^^^^^^

.. java:method:: @Override public String getName()
   :outertype: MersenneTwisterGenerator

getSeed
^^^^^^^

.. java:method:: @Override public long getSeed()
   :outertype: MersenneTwisterGenerator

nextDouble
^^^^^^^^^^

.. java:method:: @Override public double nextDouble(double lowerBound, double upperBound)
   :outertype: MersenneTwisterGenerator

nextDouble
^^^^^^^^^^

.. java:method:: @Override public double nextDouble()
   :outertype: MersenneTwisterGenerator

nextInt
^^^^^^^

.. java:method:: @Override public int nextInt(int lowerBound, int upperBound)
   :outertype: MersenneTwisterGenerator

setSeed
^^^^^^^

.. java:method:: @Override public void setSeed(long seed)
   :outertype: MersenneTwisterGenerator

