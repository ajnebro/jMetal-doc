.. java:import:: org.uma.jmetal.solution SolutionEvaluator.Objective

.. java:import:: java.lang.reflect Method

.. java:import:: java.util Collection

.. java:import:: java.util HashMap

.. java:import:: java.util LinkedList

.. java:import:: java.util Map

.. java:import:: java.util Map.Entry

ObjectiveFactory
================

.. java:package:: org.uma.jmetal.solution.impl
   :noindex:

.. java:type:: public class ObjectiveFactory

   This factory provides facilities to generate \ :java:ref:`Objective`\ s from usual situations.

   :author: Matthieu Vergne

Methods
-------
createFromGetters
^^^^^^^^^^^^^^^^^

.. java:method:: public <Solution> Collection<Objective<Solution, ?>> createFromGetters(Class<Solution> solutionClass)
   :outertype: ObjectiveFactory

   This method retrieves all the values accessible through a getter ( \ ``getX()``\  method) in order to build the corresponding set of \ :java:ref:`Objective`\ s. Notice that \ :java:ref:`Objective`\ s are supposed to represent evaluations of a \ :java:ref:`Solution`\ , so if the \ :java:ref:`Solution`\  has other kinds of information accessible through getters, they will also be retrieved as \ :java:ref:`Objective`\ s. In such a case, you should filter the returned \ :java:ref:`Objective`\ s, rely on more advanced methods, or generate the \ :java:ref:`Objective`\ s manually.

   :param solutionClass: the \ :java:ref:`Solution`\  class to analyze
   :return: the set of \ :java:ref:`Objective`\ s retrieved from this class

   **See also:** :java:ref:`.createFromLonelyGetters(Class)`

createFromGettersWithoutSetters
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public <Solution> Collection<Objective<Solution, ?>> createFromGettersWithoutSetters(Class<Solution> solutionClass)
   :outertype: ObjectiveFactory

   This method retrieves all the values accessible through a getter ( \ ``getX()``\  method) in order to build the corresponding set of \ :java:ref:`Objective`\ s. At the opposite of \ :java:ref:`createFromGetters(Class)`\ , an additional filter is used: we build an \ :java:ref:`Objective`\  for each getter which does not correspond to a setter (\ ``setX()``\  method with the same \ ``X``\  than the getter). This method is adapted for \ :java:ref:`Solution`\  implementations which provide setters only for their fundamental values (e.g. the path of a TSP \ :java:ref:`Solution`\ ) and use getters only for the computed values (e.g. the length of such a path).  Notice that, if all the relevant getters are not present, the corresponding \ :java:ref:`Objective`\ s will not be retrieved. On the opposite, any additional getter which does not correspond to a relevant \ :java:ref:`Objective`\  will be mistakenly retrieved. So be sure that the relevant elements (and only these ones) have their getter (and no setter). Otherwise, you should use a different method or generate the \ :java:ref:`Objective`\ s manually.

   :param solutionClass: the \ :java:ref:`Solution`\  class to analyze
   :return: the set of \ :java:ref:`Objective`\ s retrieved from this class

