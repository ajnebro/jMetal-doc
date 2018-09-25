.. java:import:: org.uma.jmetal.problem.impl AbstractDoubleProblem

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: java.util ArrayList

.. java:import:: java.util List

GLT4
====

.. java:package:: org.uma.jmetal.problem.multiobjective.glt
   :noindex:

.. java:type:: @SuppressWarnings public class GLT4 extends AbstractDoubleProblem

   Problem GLT4. Defined in F. Gu, H.-L. Liu, and K. C. Tan, “A multiobjective evolutionary algorithm using dynamic weight design method,” International Journal of Innovative Computing, Information and Control, vol. 8, no. 5B, pp. 3677–3688, 2012.

   :author: Antonio J. Nebro

Constructors
------------
GLT4
^^^^

.. java:constructor:: public GLT4()
   :outertype: GLT4

   Default constructor

GLT4
^^^^

.. java:constructor:: public GLT4(int numberOfVariables)
   :outertype: GLT4

   Constructor

   :param numberOfVariables:

Methods
-------
evaluate
^^^^^^^^

.. java:method:: @Override public void evaluate(DoubleSolution solution)
   :outertype: GLT4

