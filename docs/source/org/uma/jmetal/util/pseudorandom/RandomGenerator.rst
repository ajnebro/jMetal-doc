.. java:import:: java.util ArrayList

.. java:import:: java.util Arrays

.. java:import:: java.util Collection

.. java:import:: java.util.function Predicate

RandomGenerator
===============

.. java:package:: org.uma.jmetal.util.pseudorandom
   :noindex:

.. java:type:: @FunctionalInterface public interface RandomGenerator<Value>

   A \ :java:ref:`RandomGenerator`\  aims to provide a random value of a given type. Any value of this type can be generated.  A \ :java:ref:`RandomGenerator`\  is a \ :java:ref:`FunctionalInterface`\ . It is not intended to be directly implemented by a class, but instead to request a method for generating random values, usually by using lambda expressions.

   :author: Matthieu Vergne
   :param <Value>: The type of value to generate

Methods
-------
filter
^^^^^^

.. java:method:: static <T> RandomGenerator<T> filter(RandomGenerator<T> generator, Predicate<T> filter)
   :outertype: RandomGenerator

   Reduce a \ :java:ref:`RandomGenerator`\  range. The returned \ :java:ref:`RandomGenerator`\  uses the provided one to generate random values, but regenerate them if they do not pass the filter. Consequently, the initial \ :java:ref:`RandomGenerator`\  may be called several times o generate a single value. The impact on performance depends on the part of the distribution which is filtered out: if a significant part of the distribution is rejected, it might be more interesting to create a dedicated \ :java:ref:`RandomGenerator`\ .

   :param generator: the \ :java:ref:`RandomGenerator`\  to filter
   :param filter: the filter to pass to be an acceptable value
   :return: a \ :java:ref:`RandomGenerator`\  which provides only acceptable values

forArray
^^^^^^^^

.. java:method:: @SafeVarargs static <T> RandomGenerator<T> forArray(BoundedRandomGenerator<Integer> indexSelector, T... values)
   :outertype: RandomGenerator

   Create a \ :java:ref:`RandomGenerator`\  over an array based on a random selector.

   :param indexSelector: the random selector
   :param values: the values to return
   :return: a \ :java:ref:`RandomGenerator`\  on the provided values

forCollection
^^^^^^^^^^^^^

.. java:method:: static <T> RandomGenerator<T> forCollection(BoundedRandomGenerator<Integer> indexSelector, Collection<T> values)
   :outertype: RandomGenerator

   Create a \ :java:ref:`RandomGenerator`\  over a \ :java:ref:`Collection`\  based on a random selector.

   :param indexSelector: the random selector
   :param values: the values to return
   :return: a \ :java:ref:`RandomGenerator`\  on the provided values

forEnum
^^^^^^^

.. java:method:: static <T extends Enum<T>> RandomGenerator<T> forEnum(BoundedRandomGenerator<Integer> indexSelector, Class<T> enumClass)
   :outertype: RandomGenerator

   Create a \ :java:ref:`RandomGenerator`\  over \ :java:ref:`Enum`\  values based on a random selector.

   :param indexSelector: the random selector
   :param enumClass: the \ :java:ref:`Enum`\  to cover
   :return: a \ :java:ref:`RandomGenerator`\  on the \ :java:ref:`Enum`\  values

getRandomValue
^^^^^^^^^^^^^^

.. java:method:: public Value getRandomValue()
   :outertype: RandomGenerator

   Generate a random value.

   :return: the value generated

