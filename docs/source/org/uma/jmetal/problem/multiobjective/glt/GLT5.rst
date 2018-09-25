.. java:import:: org.uma.jmetal.problem.impl AbstractDoubleProblem

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: java.util ArrayList

.. java:import:: java.util List

GLT5
====

.. java:package:: org.uma.jmetal.problem.multiobjective.glt
   :noindex:

.. java:type:: @SuppressWarnings public class GLT5 extends AbstractDoubleProblem

   Problem GLT5. Defined in F. Gu, H.-L. Liu, and K. C. Tan, “A multiobjective evolutionary algorithm using dynamic weight design method,” International Journal of Innovative Computing, Information and Control, vol. 8, no. 5B, pp. 3677–3688, 2012.

   :author: Antonio J. Nebro

Constructors
------------
GLT5
^^^^

.. java:constructor:: public GLT5()
   :outertype: GLT5

   Default constructor

GLT5
^^^^

.. java:constructor:: public GLT5(int numberOfVariables)
   :outertype: GLT5

   Constructor

   :param numberOfVariables:

Methods
-------
evaluate
^^^^^^^^

.. java:method:: @Override public void evaluate(DoubleSolution solution)
   :outertype: GLT5

