.. java:import:: org.apache.commons.math3.random Well44497b

.. java:import:: org.uma.jmetal.util.pseudorandom PseudoRandomGenerator

Well44497bGenerator
===================

.. java:package:: org.uma.jmetal.util.pseudorandom.impl
   :noindex:

.. java:type:: @SuppressWarnings public class Well44497bGenerator implements PseudoRandomGenerator

   :author: Antonio J. Nebro

Constructors
------------
Well44497bGenerator
^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public Well44497bGenerator()
   :outertype: Well44497bGenerator

   Constructor

Well44497bGenerator
^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public Well44497bGenerator(long seed)
   :outertype: Well44497bGenerator

   Constructor

Methods
-------
getName
^^^^^^^

.. java:method:: @Override public String getName()
   :outertype: Well44497bGenerator

getSeed
^^^^^^^

.. java:method:: @Override public long getSeed()
   :outertype: Well44497bGenerator

nextDouble
^^^^^^^^^^

.. java:method:: @Override public double nextDouble(double lowerBound, double upperBound)
   :outertype: Well44497bGenerator

nextDouble
^^^^^^^^^^

.. java:method:: @Override public double nextDouble()
   :outertype: Well44497bGenerator

nextInt
^^^^^^^

.. java:method:: @Override public int nextInt(int lowerBound, int upperBound)
   :outertype: Well44497bGenerator

setSeed
^^^^^^^

.. java:method:: @Override public void setSeed(long seed)
   :outertype: Well44497bGenerator

