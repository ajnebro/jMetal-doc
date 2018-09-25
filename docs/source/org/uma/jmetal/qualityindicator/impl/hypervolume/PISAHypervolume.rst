.. java:import:: org.uma.jmetal.qualityindicator.impl Hypervolume

.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: org.uma.jmetal.util.comparator HypervolumeContributionComparator

.. java:import:: org.uma.jmetal.util.front Front

.. java:import:: org.uma.jmetal.util.front.imp ArrayFront

.. java:import:: org.uma.jmetal.util.front.util FrontNormalizer

.. java:import:: org.uma.jmetal.util.front.util FrontUtils

.. java:import:: org.uma.jmetal.util.point Point

.. java:import:: org.uma.jmetal.util.solutionattribute.impl HypervolumeContributionAttribute

.. java:import:: java.io FileNotFoundException

.. java:import:: java.util Collections

.. java:import:: java.util LinkedList

.. java:import:: java.util List

PISAHypervolume
===============

.. java:package:: org.uma.jmetal.qualityindicator.impl.hypervolume
   :noindex:

.. java:type:: @SuppressWarnings public class PISAHypervolume<S extends Solution<?>> extends Hypervolume<S>

   This class implements the hypervolume indicator. The code is the a Java version of the original metric implementation by Eckart Zitzler. Reference: E. Zitzler and L. Thiele Multiobjective Evolutionary Algorithms: A Comparative Case Study and the Strength Pareto Approach, IEEE Transactions on Evolutionary Computation, vol. 3, no. 4, pp. 257-271, 1999.

   :author: Antonio J. Nebro , Juan J. Durillo

Constructors
------------
PISAHypervolume
^^^^^^^^^^^^^^^

.. java:constructor:: public PISAHypervolume()
   :outertype: PISAHypervolume

   Default constructor

PISAHypervolume
^^^^^^^^^^^^^^^

.. java:constructor:: public PISAHypervolume(String referenceParetoFrontFile) throws FileNotFoundException
   :outertype: PISAHypervolume

   Constructor

   :param referenceParetoFrontFile:
   :throws FileNotFoundException:

PISAHypervolume
^^^^^^^^^^^^^^^

.. java:constructor:: public PISAHypervolume(Front referenceParetoFront)
   :outertype: PISAHypervolume

   Constructor

   :param referenceParetoFront:
   :throws FileNotFoundException:

Methods
-------
calculateHypervolume
^^^^^^^^^^^^^^^^^^^^

.. java:method:: public double calculateHypervolume(double[][] front, int noPoints, int noObjectives)
   :outertype: PISAHypervolume

computeHypervolumeContribution
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public List<S> computeHypervolumeContribution(List<S> solutionList, List<S> referenceFrontList)
   :outertype: PISAHypervolume

evaluate
^^^^^^^^

.. java:method:: @Override public Double evaluate(List<S> paretoFrontApproximation)
   :outertype: PISAHypervolume

   Evaluate() method

   :param paretoFrontApproximation:

getDescription
^^^^^^^^^^^^^^

.. java:method:: @Override public String getDescription()
   :outertype: PISAHypervolume

getOffset
^^^^^^^^^

.. java:method:: @Override public double getOffset()
   :outertype: PISAHypervolume

setOffset
^^^^^^^^^

.. java:method:: @Override public void setOffset(double offset)
   :outertype: PISAHypervolume

