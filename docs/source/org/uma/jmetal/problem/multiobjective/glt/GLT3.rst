.. java:import:: org.uma.jmetal.problem.impl AbstractDoubleProblem

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: java.util ArrayList

.. java:import:: java.util List

GLT3
====

.. java:package:: org.uma.jmetal.problem.multiobjective.glt
   :noindex:

.. java:type:: @SuppressWarnings public class GLT3 extends AbstractDoubleProblem

   Problem GLT3. Defined in F. Gu, H.-L. Liu, and K. C. Tan, “A multiobjective evolutionary algorithm using dynamic weight design method,” International Journal of Innovative Computing, Information and Control, vol. 8, no. 5B, pp. 3677–3688, 2012.

   :author: Antonio J. Nebro

Constructors
------------
GLT3
^^^^

.. java:constructor:: public GLT3()
   :outertype: GLT3

   Default constructor

GLT3
^^^^

.. java:constructor:: public GLT3(int numberOfVariables)
   :outertype: GLT3

   Constructor

   :param numberOfVariables:

Methods
-------
evaluate
^^^^^^^^

.. java:method:: @Override public void evaluate(DoubleSolution solution)
   :outertype: GLT3

