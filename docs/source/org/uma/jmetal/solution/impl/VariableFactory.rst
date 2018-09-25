.. java:import:: org.uma.jmetal.solution SolutionBuilder.Variable

.. java:import:: java.lang.reflect Constructor

.. java:import:: java.lang.reflect Method

.. java:import:: java.util Map.Entry

VariableFactory
===============

.. java:package:: org.uma.jmetal.solution.impl
   :noindex:

.. java:type:: public class VariableFactory

   This factory provides facilities to generate \ :java:ref:`Variable`\ s from usual situations.

   :author: Matthieu Vergne

Methods
-------
createFromGetters
^^^^^^^^^^^^^^^^^

.. java:method:: public <Solution> Collection<Variable<Solution, ?>> createFromGetters(Class<Solution> solutionClass)
   :outertype: VariableFactory

   This method retrieves all the values accessible through a getter ( \ ``getX()``\  method) in order to build the corresponding set of \ :java:ref:`Variable`\ s. Notice that \ :java:ref:`Variable`\ s are supposed to represent the fundamental description of a \ :java:ref:`Solution`\ , so if the \ :java:ref:`Solution`\  has computation or other additional methods which are named as getters, they will also be retrieved as \ :java:ref:`Variable`\ s. In such a case, you should filter the returned \ :java:ref:`Variable`\ s, rely on more advanced methods, or generate the \ :java:ref:`Variable`\ s manually.

   :param solutionClass: the \ :java:ref:`Solution`\  class to analyze
   :return: the set of \ :java:ref:`Variable`\ s retrieved from this class

   **See also:** :java:ref:`.createFromGettersAndSetters(Class)`, :java:ref:`.createFromGettersAndConstructors(Class)`

createFromGettersAndConstructors
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public <Solution> Collection<Variable<Solution, ?>> createFromGettersAndConstructors(Class<Solution> solutionClass)
   :outertype: VariableFactory

   This method retrieves all the values accessible through a getter ( \ ``getX()``\  method) in order to build the corresponding set of \ :java:ref:`Variable`\ s. At the opposite of \ :java:ref:`createFromGetters(Class)`\ , an additional filter is used: we build a \ :java:ref:`Variable`\  for each getter which corresponds to a constructor argument (argument of the same type). This method is adapted for static \ :java:ref:`Solution`\  implementations, which usually have a constructor which takes all the relevant values and provide getters to retrieve them.  Because Java reflection does not always provide the required information (e.g. names of constructor arguments), this method can be applied only on solution classes which meet strict constraints:

   ..

   * only one getter should return a given type
   * for each constructor and between constructors, only one argument should be of a given type (it can appear in several constructors, but it should be always the same argument)

   If all the constraints are not met, an exception will be thrown.

   :param solutionClass: the \ :java:ref:`Solution`\  class to analyze
   :throws IllegalArgumentException: if one of the constraints is not met
   :throws IsInterfaceException: if the \ :java:ref:`Solution`\  class to analyze is an interface, thus constructors make no sense
   :return: the set of \ :java:ref:`Variable`\ s retrieved from this class

createFromGettersAndSetters
^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public <Solution> Collection<Variable<Solution, ?>> createFromGettersAndSetters(Class<Solution> solutionClass)
   :outertype: VariableFactory

   This method retrieves all the values accessible through a getter ( \ ``getX()``\  method) in order to build the corresponding set of \ :java:ref:`Variable`\ s. At the opposite of \ :java:ref:`createFromGetters(Class)`\ , an additional filter is used: we build a \ :java:ref:`Variable`\  for each getter which corresponds to a setter (\ ``setX()``\  method with the same \ ``X``\  than the getter). This method is adapted for dynamic \ :java:ref:`Solution`\  implementations, thus allowing to change the value of its \ :java:ref:`Variable`\ s (e.g. change the path of a TSP \ :java:ref:`Solution`\ ).  Notice that, if all the relevant setters are not present (or they do not strictly respect the naming of the getter), the corresponding \ :java:ref:`Variable`\ s will not be retrieved. On the opposite, any additional setter/getter couple which does not correspond to a relevant \ :java:ref:`Variable`\  will be mistakenly retrieved. So be sure that the relevant elements (and only these ones) have their setter and getter. Otherwise, you should use a different method or generate the \ :java:ref:`Variable`\ s manually.

   :param solutionClass: the \ :java:ref:`Solution`\  class to analyze
   :return: the set of \ :java:ref:`Variable`\ s retrieved from this class

