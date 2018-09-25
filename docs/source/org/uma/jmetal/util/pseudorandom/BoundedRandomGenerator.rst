BoundedRandomGenerator
======================

.. java:package:: org.uma.jmetal.util.pseudorandom
   :noindex:

.. java:type:: @FunctionalInterface public interface BoundedRandomGenerator<Value extends Comparable<Value>>

   A \ :java:ref:`BoundedRandomGenerator`\  aims to provide a random value within a specific range. The range is inclusive, such that the lower bound and upper bound can be generated. Because lower and upper bounds make no sense if values cannot be compared, only \ :java:ref:`Comparable`\  values can be generated through this kind of generator.  A \ :java:ref:`BoundedRandomGenerator`\  is a \ :java:ref:`FunctionalInterface`\ . It is not intended to be directly implemented by a class, but instead to request a method for generating random values, usually by using lambda expressions.

   :author: Matthieu Vergne
   :param <Value>: The type of value to generate

Methods
-------
bound
^^^^^

.. java:method:: static BoundedRandomGenerator<Double> bound(RandomGenerator<Double> unboundedGenerator)
   :outertype: BoundedRandomGenerator

   Create a \ :java:ref:`BoundedRandomGenerator`\  from a \ :java:ref:`RandomGenerator`\  which generate \ :java:ref:`Double`\  values between 0 and 1 (inclusive or exclusive). The distribution is preserved.

   :param unboundedGenerator: \ :java:ref:`RandomGenerator`\  which generates values between 0 and 1
   :return: \ :java:ref:`BoundedRandomGenerator`\  which generates \ :java:ref:`Double`\  values based on the provided generator

fromDoubleToInteger
^^^^^^^^^^^^^^^^^^^

.. java:method:: static BoundedRandomGenerator<Integer> fromDoubleToInteger(BoundedRandomGenerator<Double> doubleGenerator)
   :outertype: BoundedRandomGenerator

   Create a \ :java:ref:`BoundedRandomGenerator`\  which generates \ :java:ref:`Integer`\  values from a \ :java:ref:`BoundedRandomGenerator`\  which generate \ :java:ref:`Double`\  values. The distribution is preserved.

   :param doubleGenerator: \ :java:ref:`BoundedRandomGenerator`\  which generates \ :java:ref:`Double`\  values
   :return: \ :java:ref:`BoundedRandomGenerator`\  which generates \ :java:ref:`Integer`\  values based on the provided generator

fromDoubleToInteger
^^^^^^^^^^^^^^^^^^^

.. java:method:: static BoundedRandomGenerator<Integer> fromDoubleToInteger(RandomGenerator<Double> doubleGenerator)
   :outertype: BoundedRandomGenerator

   Create a \ :java:ref:`BoundedRandomGenerator`\  which generates \ :java:ref:`Integer`\  values from a \ :java:ref:`BoundedRandomGenerator`\  which generate \ :java:ref:`Double`\  values between 0 and 1 (inclusive or exclusive). The distribution is preserved.

   :param doubleGenerator: \ :java:ref:`RandomGenerator`\  which generates \ :java:ref:`Double`\  values
   :return: \ :java:ref:`BoundedRandomGenerator`\  which generates \ :java:ref:`Integer`\  values based on the provided generator

getRandomValue
^^^^^^^^^^^^^^

.. java:method::  Value getRandomValue(Value lowerBound, Value upperBound)
   :outertype: BoundedRandomGenerator

   Generate a random value within the provided range.

   :param lowerBound: the minimal value which can be generated
   :param upperBound: the maximal value which can be generated
   :return: the value generated

