.. java:import:: org.uma.jmetal.operator CrossoverOperator

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: org.uma.jmetal.util JMetalLogger

.. java:import:: org.uma.jmetal.util.pseudorandom BoundedRandomGenerator

.. java:import:: org.uma.jmetal.util.pseudorandom JMetalRandom

.. java:import:: org.uma.jmetal.util.pseudorandom RandomGenerator

.. java:import:: java.util ArrayList

.. java:import:: java.util List

DifferentialEvolutionCrossover
==============================

.. java:package:: org.uma.jmetal.operator.impl.crossover
   :noindex:

.. java:type:: @SuppressWarnings public class DifferentialEvolutionCrossover implements CrossoverOperator<DoubleSolution>

   Differential evolution crossover operator

   :author: Antonio J. Nebro Comments: - The operator receives two parameters: the current individual and an array of three parent individuals - The best and rand variants depends on the third parent, according whether it represents the current of the "best" individual or a random one. The implementation of both variants are the same, due to that the parent selection is external to the crossover operator. - Implemented variants: - rand/1/bin (best/1/bin) - rand/1/exp (best/1/exp) - current-to-rand/1 (current-to-best/1) - current-to-rand/1/bin (current-to-best/1/bin) - current-to-rand/1/exp (current-to-best/1/exp)

Constructors
------------
DifferentialEvolutionCrossover
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public DifferentialEvolutionCrossover()
   :outertype: DifferentialEvolutionCrossover

   Constructor

DifferentialEvolutionCrossover
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public DifferentialEvolutionCrossover(double cr, double f, String variant)
   :outertype: DifferentialEvolutionCrossover

   Constructor

   :param cr:
   :param f:
   :param variant:

DifferentialEvolutionCrossover
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public DifferentialEvolutionCrossover(double cr, double f, String variant, RandomGenerator<Double> randomGenerator)
   :outertype: DifferentialEvolutionCrossover

   Constructor

   :param cr:
   :param f:
   :param variant:
   :param jRandomGenerator:
   :param crRandomGenerator:

DifferentialEvolutionCrossover
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public DifferentialEvolutionCrossover(double cr, double f, String variant, BoundedRandomGenerator<Integer> jRandomGenerator, BoundedRandomGenerator<Double> crRandomGenerator)
   :outertype: DifferentialEvolutionCrossover

   Constructor

   :param cr:
   :param f:
   :param variant:
   :param jRandomGenerator:
   :param crRandomGenerator:

DifferentialEvolutionCrossover
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public DifferentialEvolutionCrossover(double cr, double f, double k, String variant)
   :outertype: DifferentialEvolutionCrossover

   Constructor

Methods
-------
execute
^^^^^^^

.. java:method:: @Override public List<DoubleSolution> execute(List<DoubleSolution> parentSolutions)
   :outertype: DifferentialEvolutionCrossover

   Execute() method

getCr
^^^^^

.. java:method:: public double getCr()
   :outertype: DifferentialEvolutionCrossover

getF
^^^^

.. java:method:: public double getF()
   :outertype: DifferentialEvolutionCrossover

getK
^^^^

.. java:method:: public double getK()
   :outertype: DifferentialEvolutionCrossover

getNumberOfGeneratedChildren
^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public int getNumberOfGeneratedChildren()
   :outertype: DifferentialEvolutionCrossover

getNumberOfRequiredParents
^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public int getNumberOfRequiredParents()
   :outertype: DifferentialEvolutionCrossover

getVariant
^^^^^^^^^^

.. java:method:: public String getVariant()
   :outertype: DifferentialEvolutionCrossover

setCr
^^^^^

.. java:method:: public void setCr(double cr)
   :outertype: DifferentialEvolutionCrossover

setCurrentSolution
^^^^^^^^^^^^^^^^^^

.. java:method:: public void setCurrentSolution(DoubleSolution current)
   :outertype: DifferentialEvolutionCrossover

setF
^^^^

.. java:method:: public void setF(double f)
   :outertype: DifferentialEvolutionCrossover

setK
^^^^

.. java:method:: public void setK(double k)
   :outertype: DifferentialEvolutionCrossover

