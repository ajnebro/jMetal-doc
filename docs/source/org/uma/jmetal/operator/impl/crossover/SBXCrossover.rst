.. java:import:: org.uma.jmetal.operator CrossoverOperator

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.solution.util RepairDoubleSolution

.. java:import:: org.uma.jmetal.solution.util RepairDoubleSolutionAtBounds

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: org.uma.jmetal.util.pseudorandom JMetalRandom

.. java:import:: org.uma.jmetal.util.pseudorandom RandomGenerator

.. java:import:: java.util ArrayList

.. java:import:: java.util List

SBXCrossover
============

.. java:package:: org.uma.jmetal.operator.impl.crossover
   :noindex:

.. java:type:: @SuppressWarnings public class SBXCrossover implements CrossoverOperator<DoubleSolution>

   This class allows to apply a SBX crossover operator using two parent solutions (Double encoding). A \ :java:ref:`RepairDoubleSolution`\  object is used to decide the strategy to apply when a value is out of range. The implementation is based on the NSGA-II code available in \ `http://www.iitk.ac.in/kangal/codes.shtml <http://www.iitk.ac.in/kangal/codes.shtml>`_\

   :author: Antonio J. Nebro , Juan J. Durillo

Constructors
------------
SBXCrossover
^^^^^^^^^^^^

.. java:constructor:: public SBXCrossover(double crossoverProbability, double distributionIndex)
   :outertype: SBXCrossover

   Constructor

SBXCrossover
^^^^^^^^^^^^

.. java:constructor:: public SBXCrossover(double crossoverProbability, double distributionIndex, RandomGenerator<Double> randomGenerator)
   :outertype: SBXCrossover

   Constructor

SBXCrossover
^^^^^^^^^^^^

.. java:constructor:: public SBXCrossover(double crossoverProbability, double distributionIndex, RepairDoubleSolution solutionRepair)
   :outertype: SBXCrossover

   Constructor

SBXCrossover
^^^^^^^^^^^^

.. java:constructor:: public SBXCrossover(double crossoverProbability, double distributionIndex, RepairDoubleSolution solutionRepair, RandomGenerator<Double> randomGenerator)
   :outertype: SBXCrossover

   Constructor

Methods
-------
doCrossover
^^^^^^^^^^^

.. java:method:: public List<DoubleSolution> doCrossover(double probability, DoubleSolution parent1, DoubleSolution parent2)
   :outertype: SBXCrossover

   doCrossover method

execute
^^^^^^^

.. java:method:: @Override public List<DoubleSolution> execute(List<DoubleSolution> solutions)
   :outertype: SBXCrossover

   Execute() method

getCrossoverProbability
^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public double getCrossoverProbability()
   :outertype: SBXCrossover

getDistributionIndex
^^^^^^^^^^^^^^^^^^^^

.. java:method:: public double getDistributionIndex()
   :outertype: SBXCrossover

getNumberOfGeneratedChildren
^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public int getNumberOfGeneratedChildren()
   :outertype: SBXCrossover

getNumberOfRequiredParents
^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public int getNumberOfRequiredParents()
   :outertype: SBXCrossover

setCrossoverProbability
^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public void setCrossoverProbability(double probability)
   :outertype: SBXCrossover

setDistributionIndex
^^^^^^^^^^^^^^^^^^^^

.. java:method:: public void setDistributionIndex(double distributionIndex)
   :outertype: SBXCrossover

