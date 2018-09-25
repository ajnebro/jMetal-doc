.. java:import:: org.uma.jmetal.algorithm.impl AbstractEvolutionStrategy

.. java:import:: org.uma.jmetal.algorithm.singleobjective.evolutionstrategy.util CMAESUtils

.. java:import:: org.uma.jmetal.problem DoubleProblem

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.util JMetalLogger

.. java:import:: org.uma.jmetal.util.comparator ObjectiveComparator

CovarianceMatrixAdaptationEvolutionStrategy
===========================================

.. java:package:: org.uma.jmetal.algorithm.singleobjective.evolutionstrategy
   :noindex:

.. java:type:: @SuppressWarnings public class CovarianceMatrixAdaptationEvolutionStrategy extends AbstractEvolutionStrategy<DoubleSolution, DoubleSolution>

   Class implementing the CMA-ES algorithm

Methods
-------
createInitialPopulation
^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override protected List<DoubleSolution> createInitialPopulation()
   :outertype: CovarianceMatrixAdaptationEvolutionStrategy

evaluatePopulation
^^^^^^^^^^^^^^^^^^

.. java:method:: @Override protected List<DoubleSolution> evaluatePopulation(List<DoubleSolution> population)
   :outertype: CovarianceMatrixAdaptationEvolutionStrategy

getDescription
^^^^^^^^^^^^^^

.. java:method:: @Override public String getDescription()
   :outertype: CovarianceMatrixAdaptationEvolutionStrategy

getLambda
^^^^^^^^^

.. java:method:: public int getLambda()
   :outertype: CovarianceMatrixAdaptationEvolutionStrategy

getMaxEvaluations
^^^^^^^^^^^^^^^^^

.. java:method:: public int getMaxEvaluations()
   :outertype: CovarianceMatrixAdaptationEvolutionStrategy

getName
^^^^^^^

.. java:method:: @Override public String getName()
   :outertype: CovarianceMatrixAdaptationEvolutionStrategy

getResult
^^^^^^^^^

.. java:method:: @Override public DoubleSolution getResult()
   :outertype: CovarianceMatrixAdaptationEvolutionStrategy

initProgress
^^^^^^^^^^^^

.. java:method:: @Override protected void initProgress()
   :outertype: CovarianceMatrixAdaptationEvolutionStrategy

isStoppingConditionReached
^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override protected boolean isStoppingConditionReached()
   :outertype: CovarianceMatrixAdaptationEvolutionStrategy

replacement
^^^^^^^^^^^

.. java:method:: @Override protected List<DoubleSolution> replacement(List<DoubleSolution> population, List<DoubleSolution> offspringPopulation)
   :outertype: CovarianceMatrixAdaptationEvolutionStrategy

reproduction
^^^^^^^^^^^^

.. java:method:: @Override protected List<DoubleSolution> reproduction(List<DoubleSolution> population)
   :outertype: CovarianceMatrixAdaptationEvolutionStrategy

selection
^^^^^^^^^

.. java:method:: @Override protected List<DoubleSolution> selection(List<DoubleSolution> population)
   :outertype: CovarianceMatrixAdaptationEvolutionStrategy

updateProgress
^^^^^^^^^^^^^^

.. java:method:: @Override protected void updateProgress()
   :outertype: CovarianceMatrixAdaptationEvolutionStrategy

