.. java:import:: org.uma.jmetal.problem.impl AbstractDoubleProblem

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: java.util ArrayList

.. java:import:: java.util List

MOP3
====

.. java:package:: org.uma.jmetal.problem.multiobjective.mop
   :noindex:

.. java:type:: @SuppressWarnings public class MOP3 extends AbstractDoubleProblem

   Problem MOP3. Defined in H. L. Liu, F. Gu and Q. Zhang, "Decomposition of a Multiobjective Optimization Problem Into a Number of Simple Multiobjective Subproblems," in IEEE Transactions on Evolutionary Computation, vol. 18, no. 3, pp. 450-455, June 2014.

   :author: Mastermay

Constructors
------------
MOP3
^^^^

.. java:constructor:: public MOP3()
   :outertype: MOP3

   Constructor. Creates default instance of problem MOP3 (10 decision variables)

MOP3
^^^^

.. java:constructor:: public MOP3(Integer numberOfVariables)
   :outertype: MOP3

   Creates a new instance of problem MOP3.

   :param numberOfVariables: Number of variables.

Methods
-------
evaluate
^^^^^^^^

.. java:method:: public void evaluate(DoubleSolution solution)
   :outertype: MOP3

   Evaluate() method

