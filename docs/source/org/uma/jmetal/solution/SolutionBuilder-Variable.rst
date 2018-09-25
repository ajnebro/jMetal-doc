.. java:import:: org.uma.jmetal.algorithm Algorithm

.. java:import:: org.uma.jmetal.util.naming DescribedEntity

.. java:import:: java.util Collection

SolutionBuilder.Variable
========================

.. java:package:: org.uma.jmetal.solution
   :noindex:

.. java:type:: public static interface Variable<Solution, Value> extends DescribedEntity
   :outertype: SolutionBuilder

   A \ :java:ref:`Variable`\  represents the fundamental information of a set of homogeneous \ :java:ref:`Solution`\ s (e.g. a population of solutions returned by an \ :java:ref:`Algorithm`\ ). For instance, an \ :java:ref:`Algorithm`\  used to solve a TSP problem would manage a whole population of \ :java:ref:`Solution`\ s, each representing a different path, and a \ :java:ref:`Variable`\  would represent a type of information which defines these \ :java:ref:`Solution`\ s, like the path they represent or something more fine grained like the i\ :sup:`th`\  city.

   :author: Matthieu Vergne
   :param <Solution>:
   :param <Value>:

Methods
-------
get
^^^

.. java:method:: public Value get(Solution solution)
   :outertype: SolutionBuilder.Variable

   :param solution: the \ :java:ref:`Solution`\  to read
   :return: the \ :java:ref:`Value`\  of the \ :java:ref:`Variable`\  for this \ :java:ref:`Solution`\

