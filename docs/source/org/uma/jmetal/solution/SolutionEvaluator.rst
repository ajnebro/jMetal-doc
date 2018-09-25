.. java:import:: org.uma.jmetal.algorithm Algorithm

.. java:import:: org.uma.jmetal.util.naming DescribedEntity

.. java:import:: java.util Collection

SolutionEvaluator
=================

.. java:package:: org.uma.jmetal.solution
   :noindex:

.. java:type:: public interface SolutionEvaluator<Solution>

   A \ :java:ref:`SolutionEvaluator`\  allows to evaluate a \ :java:ref:`Solution`\  on one or several dimensions, in other words to compute its \ :java:ref:`Objective`\  values.

   :author: Matthieu Vergne
   :param <Solution>:

Methods
-------
getObjectives
^^^^^^^^^^^^^

.. java:method:: public Collection<Objective<Solution, ?>> getObjectives()
   :outertype: SolutionEvaluator

   :return: the list of \ :java:ref:`Objective`\ s managed by this \ :java:ref:`SolutionEvaluator`\

