.. java:import:: org.uma.jmetal.problem.impl AbstractDoubleProblem

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: java.util ArrayList

.. java:import:: java.util List

GLT2
====

.. java:package:: org.uma.jmetal.problem.multiobjective.glt
   :noindex:

.. java:type:: @SuppressWarnings public class GLT2 extends AbstractDoubleProblem

   Problem GLT2. Defined in F. Gu, H.-L. Liu, and K. C. Tan, “A multiobjective evolutionary algorithm using dynamic weight design method,” International Journal of Innovative Computing, Information and Control, vol. 8, no. 5B, pp. 3677–3688, 2012.

   :author: Antonio J. Nebro

Constructors
------------
GLT2
^^^^

.. java:constructor:: public GLT2()
   :outertype: GLT2

   Default constructor

GLT2
^^^^

.. java:constructor:: public GLT2(int numberOfVariables)
   :outertype: GLT2

   Constructor

   :param numberOfVariables:

Methods
-------
evaluate
^^^^^^^^

.. java:method:: @Override public void evaluate(DoubleSolution solution)
   :outertype: GLT2

