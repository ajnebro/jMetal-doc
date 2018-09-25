.. java:import:: java.util List

.. java:import:: org.uma.jmetal.algorithm.multiobjective.moead.util MOEADUtils

.. java:import:: org.uma.jmetal.operator CrossoverOperator

.. java:import:: org.uma.jmetal.operator MutationOperator

.. java:import:: org.uma.jmetal.operator.impl.crossover DifferentialEvolutionCrossover

.. java:import:: org.uma.jmetal.operator.impl.mutation CDGMutation

.. java:import:: org.uma.jmetal.problem Problem

.. java:import:: org.uma.jmetal.solution DoubleSolution

CDG
===

.. java:package:: org.uma.jmetal.algorithm.multiobjective.cdg
   :noindex:

.. java:type:: @SuppressWarnings public class CDG extends AbstractCDG<DoubleSolution>

   Xinye Cai, Zhiwei Mei, Zhun Fan, Qingfu Zhang, A Constrained Decomposition Approach with Grids for Evolutionary Multiobjective Optimization, IEEE Transaction on Evolutionary Computation, press online, 2018, DOI: 10.1109/TEVC.2017.2744674 The paper and Matlab code can be download at http://xinyecai.github.io/

   :author: Feng Zhang

Constructors
------------
CDG
^^^

.. java:constructor:: public CDG(Problem<DoubleSolution> problem, int populationSize, int resultPopulationSize, int maxEvaluations, CrossoverOperator<DoubleSolution> crossover, double neighborhoodSelectionProbability, double sigma_, int k_, int t_, int subproblemNum_, int childGrid_, int childGridNum_)
   :outertype: CDG

Methods
-------
getDescription
^^^^^^^^^^^^^^

.. java:method:: @Override public String getDescription()
   :outertype: CDG

getName
^^^^^^^

.. java:method:: @Override public String getName()
   :outertype: CDG

initializePopulation
^^^^^^^^^^^^^^^^^^^^

.. java:method:: protected void initializePopulation()
   :outertype: CDG

run
^^^

.. java:method:: @Override public void run()
   :outertype: CDG

