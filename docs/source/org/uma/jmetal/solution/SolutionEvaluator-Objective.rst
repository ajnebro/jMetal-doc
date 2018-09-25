.. java:import:: org.uma.jmetal.algorithm Algorithm

.. java:import:: org.uma.jmetal.util.naming DescribedEntity

.. java:import:: java.util Collection

SolutionEvaluator.Objective
===========================

.. java:package:: org.uma.jmetal.solution
   :noindex:

.. java:type:: public static interface Objective<Solution, Value> extends DescribedEntity
   :outertype: SolutionEvaluator

   An \ :java:ref:`Objective`\  represents the evaluation information of a set of homogeneous \ :java:ref:`Solution`\ s (e.g. a population of solutions returned by an \ :java:ref:`Algorithm`\ ). For instance, an \ :java:ref:`Algorithm`\  used to solve a TSP problem would manage a whole population of \ :java:ref:`Solution`\ s, each representing a different path, and an \ :java:ref:`Objective`\  would represent a type of information which evaluates these \ :java:ref:`Solution`\ s, like the length of the path, the time needed to travel through this path, or the amount of fuel consumed.

   :author: Matthieu Vergne
   :param <Solution>:
   :param <Value>:

Methods
-------
get
^^^

.. java:method:: public Value get(Solution solution)
   :outertype: SolutionEvaluator.Objective

   :param solution: the \ :java:ref:`Solution`\  to read
   :return: the \ :java:ref:`Value`\  of the \ :java:ref:`Objective`\  for this \ :java:ref:`Solution`\

