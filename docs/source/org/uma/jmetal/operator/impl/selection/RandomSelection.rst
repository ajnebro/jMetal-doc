.. java:import:: org.uma.jmetal.operator SelectionOperator

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: org.uma.jmetal.util SolutionListUtils

.. java:import:: java.util List

RandomSelection
===============

.. java:package:: org.uma.jmetal.operator.impl.selection
   :noindex:

.. java:type:: @SuppressWarnings public class RandomSelection<S> implements SelectionOperator<List<S>, S>

   This class implements a random selection operator used for selecting a N number of solutions from a list

   :author: Antonio J. Nebro

Methods
-------
execute
^^^^^^^

.. java:method:: public S execute(List<S> solutionList)
   :outertype: RandomSelection

   Execute() method

