.. java:import:: org.uma.jmetal.operator CrossoverOperator

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.solution.util RepairDoubleSolution

.. java:import:: org.uma.jmetal.solution.util RepairDoubleSolutionAtBounds

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: org.uma.jmetal.util.pseudorandom JMetalRandom

.. java:import:: org.uma.jmetal.util.pseudorandom RandomGenerator

.. java:import:: java.util ArrayList

.. java:import:: java.util List

BLXAlphaCrossover
=================

.. java:package:: org.uma.jmetal.operator.impl.crossover
   :noindex:

.. java:type:: @SuppressWarnings public class BLXAlphaCrossover implements CrossoverOperator<DoubleSolution>

   This class allows to apply a BLX-alpha crossover operator to two parent solutions.

   :author: Antonio J. Nebro

Constructors
------------
BLXAlphaCrossover
^^^^^^^^^^^^^^^^^

.. java:constructor:: public BLXAlphaCrossover(double crossoverProbability)
   :outertype: BLXAlphaCrossover

   Constructor

BLXAlphaCrossover
^^^^^^^^^^^^^^^^^

.. java:constructor:: public BLXAlphaCrossover(double crossoverProbability, double alpha)
   :outertype: BLXAlphaCrossover

   Constructor

BLXAlphaCrossover
^^^^^^^^^^^^^^^^^

.. java:constructor:: public BLXAlphaCrossover(double crossoverProbability, double alpha, RepairDoubleSolution solutionRepair)
   :outertype: BLXAlphaCrossover

   Constructor

BLXAlphaCrossover
^^^^^^^^^^^^^^^^^

.. java:constructor:: public BLXAlphaCrossover(double crossoverProbability, double alpha, RepairDoubleSolution solutionRepair, RandomGenerator<Double> randomGenerator)
   :outertype: BLXAlphaCrossover

   Constructor

Methods
-------
doCrossover
^^^^^^^^^^^

.. java:method:: public List<DoubleSolution> doCrossover(double probability, DoubleSolution parent1, DoubleSolution parent2)
   :outertype: BLXAlphaCrossover

   doCrossover method

execute
^^^^^^^

.. java:method:: @Override public List<DoubleSolution> execute(List<DoubleSolution> solutions)
   :outertype: BLXAlphaCrossover

   Execute() method

getAlpha
^^^^^^^^

.. java:method:: public double getAlpha()
   :outertype: BLXAlphaCrossover

getCrossoverProbability
^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public double getCrossoverProbability()
   :outertype: BLXAlphaCrossover

getNumberOfGeneratedChildren
^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public int getNumberOfGeneratedChildren()
   :outertype: BLXAlphaCrossover

getNumberOfRequiredParents
^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public int getNumberOfRequiredParents()
   :outertype: BLXAlphaCrossover

setAlpha
^^^^^^^^

.. java:method:: public void setAlpha(double alpha)
   :outertype: BLXAlphaCrossover

setCrossoverProbability
^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public void setCrossoverProbability(double crossoverProbability)
   :outertype: BLXAlphaCrossover

