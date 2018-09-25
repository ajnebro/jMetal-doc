.. java:import:: org.uma.jmetal.algorithm.impl AbstractEvolutionStrategy

.. java:import:: org.uma.jmetal.algorithm.singleobjective.evolutionstrategy.util CMAESUtils

.. java:import:: org.uma.jmetal.problem DoubleProblem

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.util JMetalLogger

.. java:import:: org.uma.jmetal.util.comparator ObjectiveComparator

CovarianceMatrixAdaptationEvolutionStrategy.Builder
===================================================

.. java:package:: org.uma.jmetal.algorithm.singleobjective.evolutionstrategy
   :noindex:

.. java:type:: public static class Builder
   :outertype: CovarianceMatrixAdaptationEvolutionStrategy

   Buider class

Constructors
------------
Builder
^^^^^^^

.. java:constructor:: public Builder(DoubleProblem problem)
   :outertype: CovarianceMatrixAdaptationEvolutionStrategy.Builder

Methods
-------
build
^^^^^

.. java:method:: public CovarianceMatrixAdaptationEvolutionStrategy build()
   :outertype: CovarianceMatrixAdaptationEvolutionStrategy.Builder

setLambda
^^^^^^^^^

.. java:method:: public Builder setLambda(int lambda)
   :outertype: CovarianceMatrixAdaptationEvolutionStrategy.Builder

setMaxEvaluations
^^^^^^^^^^^^^^^^^

.. java:method:: public Builder setMaxEvaluations(int maxEvaluations)
   :outertype: CovarianceMatrixAdaptationEvolutionStrategy.Builder

setSigma
^^^^^^^^

.. java:method:: public Builder setSigma(double sigma)
   :outertype: CovarianceMatrixAdaptationEvolutionStrategy.Builder

setTypicalX
^^^^^^^^^^^

.. java:method:: public Builder setTypicalX(double[] typicalX)
   :outertype: CovarianceMatrixAdaptationEvolutionStrategy.Builder

