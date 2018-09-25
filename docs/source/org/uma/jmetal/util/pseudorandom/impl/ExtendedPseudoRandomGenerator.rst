.. java:import:: org.uma.jmetal.util.pseudorandom PseudoRandomGenerator

ExtendedPseudoRandomGenerator
=============================

.. java:package:: org.uma.jmetal.util.pseudorandom.impl
   :noindex:

.. java:type:: @SuppressWarnings public class ExtendedPseudoRandomGenerator implements PseudoRandomGenerator

   Extended pseudo random number generator based on the decorator pattern. Two new methods are added: randNormal() and randSphere()

   :author: Antonio J. Nebro

Constructors
------------
ExtendedPseudoRandomGenerator
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public ExtendedPseudoRandomGenerator(PseudoRandomGenerator randomGenerator)
   :outertype: ExtendedPseudoRandomGenerator

Methods
-------
getName
^^^^^^^

.. java:method:: @Override public String getName()
   :outertype: ExtendedPseudoRandomGenerator

getSeed
^^^^^^^

.. java:method:: @Override public long getSeed()
   :outertype: ExtendedPseudoRandomGenerator

nextDouble
^^^^^^^^^^

.. java:method:: @Override public double nextDouble(double lowerBound, double upperBound)
   :outertype: ExtendedPseudoRandomGenerator

nextDouble
^^^^^^^^^^

.. java:method:: @Override public double nextDouble()
   :outertype: ExtendedPseudoRandomGenerator

nextInt
^^^^^^^

.. java:method:: @Override public int nextInt(int lowerBound, int upperBound)
   :outertype: ExtendedPseudoRandomGenerator

randNormal
^^^^^^^^^^

.. java:method:: public double randNormal(double mean, double standardDeviation)
   :outertype: ExtendedPseudoRandomGenerator

   Use the polar form of the Box-Muller transformation to obtain a pseudo random number from a Gaussian distribution Code taken from Maurice Clerc's implementation

   :param mean:
   :param standardDeviation:
   :return: A pseudo random number

randSphere
^^^^^^^^^^

.. java:method:: public double[] randSphere(int dimension)
   :outertype: ExtendedPseudoRandomGenerator

   Get a random point from an hypersphere (center = 0, radius = 1) Code taken from Maurice Clerc's implementation

   :param dimension:
   :return: A pseudo random point

randSphere
^^^^^^^^^^

.. java:method:: public double[] randSphere(int dimension, double center, double radius)
   :outertype: ExtendedPseudoRandomGenerator

   Ger a random point from an hypersphere Code taken from Maurice Clerc's implementation

   :param center:
   :param radius:
   :return: A pseudo random number

setSeed
^^^^^^^

.. java:method:: @Override public void setSeed(long seed)
   :outertype: ExtendedPseudoRandomGenerator

