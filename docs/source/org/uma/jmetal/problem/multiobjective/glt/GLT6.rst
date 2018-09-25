.. java:import:: org.uma.jmetal.problem.impl AbstractDoubleProblem

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: java.util ArrayList

.. java:import:: java.util List

GLT6
====

.. java:package:: org.uma.jmetal.problem.multiobjective.glt
   :noindex:

.. java:type:: @SuppressWarnings public class GLT6 extends AbstractDoubleProblem

   Problem GLT6. Defined in F. Gu, H.-L. Liu, and K. C. Tan, “A multiobjective evolutionary algorithm using dynamic weight design method,” International Journal of Innovative Computing, Information and Control, vol. 8, no. 5B, pp. 3677–3688, 2012.

   :author: Antonio J. Nebro

Constructors
------------
GLT6
^^^^

.. java:constructor:: public GLT6()
   :outertype: GLT6

   Default constructor

GLT6
^^^^

.. java:constructor:: public GLT6(int numberOfVariables)
   :outertype: GLT6

   Constructor

   :param numberOfVariables:

Methods
-------
evaluate
^^^^^^^^

.. java:method:: @Override public void evaluate(DoubleSolution solution)
   :outertype: GLT6

