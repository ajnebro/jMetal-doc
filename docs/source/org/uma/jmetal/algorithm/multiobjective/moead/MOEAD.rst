.. java:import:: org.uma.jmetal.algorithm.multiobjective.moead.util MOEADUtils

.. java:import:: org.uma.jmetal.operator CrossoverOperator

.. java:import:: org.uma.jmetal.operator MutationOperator

.. java:import:: org.uma.jmetal.operator.impl.crossover DifferentialEvolutionCrossover

.. java:import:: org.uma.jmetal.problem Problem

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: java.util ArrayList

.. java:import:: java.util List

MOEAD
=====

.. java:package:: org.uma.jmetal.algorithm.multiobjective.moead
   :noindex:

.. java:type:: @SuppressWarnings public class MOEAD extends AbstractMOEAD<DoubleSolution>

   Class implementing the MOEA/D-DE algorithm described in : Hui Li; Qingfu Zhang, "Multiobjective Optimization Problems With Complicated Pareto Sets, MOEA/D and NSGA-II," Evolutionary Computation, IEEE Transactions on , vol.13, no.2, pp.284,302, April 2009. doi: 10.1109/TEVC.2008.925798

   :author: Antonio J. Nebro

Fields
------
differentialEvolutionCrossover
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:field:: protected DifferentialEvolutionCrossover differentialEvolutionCrossover
   :outertype: MOEAD

Constructors
------------
MOEAD
^^^^^

.. java:constructor:: public MOEAD(Problem<DoubleSolution> problem, int populationSize, int resultPopulationSize, int maxEvaluations, MutationOperator<DoubleSolution> mutation, CrossoverOperator<DoubleSolution> crossover, FunctionType functionType, String dataDirectory, double neighborhoodSelectionProbability, int maximumNumberOfReplacedSolutions, int neighborSize)
   :outertype: MOEAD

Methods
-------
getDescription
^^^^^^^^^^^^^^

.. java:method:: @Override public String getDescription()
   :outertype: MOEAD

getName
^^^^^^^

.. java:method:: @Override public String getName()
   :outertype: MOEAD

initializePopulation
^^^^^^^^^^^^^^^^^^^^

.. java:method:: protected void initializePopulation()
   :outertype: MOEAD

run
^^^

.. java:method:: @Override public void run()
   :outertype: MOEAD

