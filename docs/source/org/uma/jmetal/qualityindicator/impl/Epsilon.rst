.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: org.uma.jmetal.util.front Front

.. java:import:: org.uma.jmetal.util.front.imp ArrayFront

.. java:import:: java.io FileNotFoundException

.. java:import:: java.util List

Epsilon
=======

.. java:package:: org.uma.jmetal.qualityindicator.impl
   :noindex:

.. java:type:: @SuppressWarnings public class Epsilon<S extends Solution<?>> extends GenericIndicator<S>

   This class implements the unary epsilon additive indicator as proposed in E. Zitzler, E. Thiele, L. Laummanns, M., Fonseca, C., and Grunert da Fonseca. V (2003): Performance Assessment of Multiobjective Optimizers: An Analysis and Review. The code is the a Java version of the original metric implementation by Eckart Zitzler. It can be used also as a command line program just by typing $java org.uma.jmetal.qualityindicator.impl.Epsilon

   :author: Antonio J. Nebro , Juan J. Durillo

Constructors
------------
Epsilon
^^^^^^^

.. java:constructor:: public Epsilon()
   :outertype: Epsilon

   Default constructor

Epsilon
^^^^^^^

.. java:constructor:: public Epsilon(String referenceParetoFrontFile) throws FileNotFoundException
   :outertype: Epsilon

   Constructor

   :param referenceParetoFrontFile:
   :throws FileNotFoundException:

Epsilon
^^^^^^^

.. java:constructor:: public Epsilon(Front referenceParetoFront)
   :outertype: Epsilon

   Constructor

   :param referenceParetoFront:

Methods
-------
evaluate
^^^^^^^^

.. java:method:: @Override public Double evaluate(List<S> solutionList)
   :outertype: Epsilon

   Evaluate() method

   :param solutionList:

getDescription
^^^^^^^^^^^^^^

.. java:method:: @Override public String getDescription()
   :outertype: Epsilon

getName
^^^^^^^

.. java:method:: @Override public String getName()
   :outertype: Epsilon

isTheLowerTheIndicatorValueTheBetter
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public boolean isTheLowerTheIndicatorValueTheBetter()
   :outertype: Epsilon

