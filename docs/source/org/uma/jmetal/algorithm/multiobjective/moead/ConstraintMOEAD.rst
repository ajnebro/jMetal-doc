.. java:import:: org.uma.jmetal.algorithm.multiobjective.moead.util MOEADUtils

.. java:import:: org.uma.jmetal.operator CrossoverOperator

.. java:import:: org.uma.jmetal.operator MutationOperator

.. java:import:: org.uma.jmetal.operator.impl.crossover DifferentialEvolutionCrossover

.. java:import:: org.uma.jmetal.problem ConstrainedProblem

.. java:import:: org.uma.jmetal.problem Problem

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.util.comparator.impl ViolationThresholdComparator

.. java:import:: java.util List

ConstraintMOEAD
===============

.. java:package:: org.uma.jmetal.algorithm.multiobjective.moead
   :noindex:

.. java:type:: @SuppressWarnings public class ConstraintMOEAD extends AbstractMOEAD<DoubleSolution>

   This class implements a constrained version of the MOEAD algorithm based on the one presented in the paper: "An adaptive constraint handling approach embedded MOEA/D". DOI: 10.1109/CEC.2012.6252868

   :author: Antonio J. Nebro, Juan J. Durillo

Constructors
------------
ConstraintMOEAD
^^^^^^^^^^^^^^^

.. java:constructor:: public ConstraintMOEAD(Problem<DoubleSolution> problem, int populationSize, int resultPopulationSize, int maxEvaluations, MutationOperator<DoubleSolution> mutation, CrossoverOperator<DoubleSolution> crossover, FunctionType functionType, String dataDirectory, double neighborhoodSelectionProbability, int maximumNumberOfReplacedSolutions, int neighborSize)
   :outertype: ConstraintMOEAD

Methods
-------
getDescription
^^^^^^^^^^^^^^

.. java:method:: @Override public String getDescription()
   :outertype: ConstraintMOEAD

getName
^^^^^^^

.. java:method:: @Override public String getName()
   :outertype: ConstraintMOEAD

initializePopulation
^^^^^^^^^^^^^^^^^^^^

.. java:method:: public void initializePopulation()
   :outertype: ConstraintMOEAD

run
^^^

.. java:method:: @Override public void run()
   :outertype: ConstraintMOEAD

updateNeighborhood
^^^^^^^^^^^^^^^^^^

.. java:method:: @Override protected void updateNeighborhood(DoubleSolution individual, int subproblemId, NeighborType neighborType)
   :outertype: ConstraintMOEAD

