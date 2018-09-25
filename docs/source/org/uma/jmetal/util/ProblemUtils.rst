.. java:import:: org.uma.jmetal.problem Problem

.. java:import:: java.lang.reflect InvocationTargetException

ProblemUtils
============

.. java:package:: org.uma.jmetal.util
   :noindex:

.. java:type:: public class ProblemUtils

   :author: Antonio J. Nebro

Methods
-------
loadProblem
^^^^^^^^^^^

.. java:method:: @SuppressWarnings public static <S> Problem<S> loadProblem(String problemName)
   :outertype: ProblemUtils

   Create an instance of problem passed as argument

   :param problemName: A full qualified problem name
   :return: An instance of the problem

