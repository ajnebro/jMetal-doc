.. java:import:: org.uma.jmetal.algorithm Algorithm

.. java:import:: org.uma.jmetal.operator MutationOperator

.. java:import:: org.uma.jmetal.problem Problem

.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util AlgorithmBuilder

.. java:import:: org.uma.jmetal.util JMetalException

EvolutionStrategyBuilder
========================

.. java:package:: org.uma.jmetal.algorithm.singleobjective.evolutionstrategy
   :noindex:

.. java:type:: public class EvolutionStrategyBuilder<S extends Solution<?>> implements AlgorithmBuilder<Algorithm<S>>

   Class implementing a (mu , lambda) Evolution Strategy (lambda must be divisible by mu)

   :author: Antonio J. Nebro

Constructors
------------
EvolutionStrategyBuilder
^^^^^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public EvolutionStrategyBuilder(Problem<S> problem, MutationOperator<S> mutationOperator, EvolutionStrategyVariant variant)
   :outertype: EvolutionStrategyBuilder

Methods
-------
build
^^^^^

.. java:method:: @Override public Algorithm<S> build()
   :outertype: EvolutionStrategyBuilder

getLambda
^^^^^^^^^

.. java:method:: public int getLambda()
   :outertype: EvolutionStrategyBuilder

getMaxEvaluations
^^^^^^^^^^^^^^^^^

.. java:method:: public int getMaxEvaluations()
   :outertype: EvolutionStrategyBuilder

getMu
^^^^^

.. java:method:: public int getMu()
   :outertype: EvolutionStrategyBuilder

getMutation
^^^^^^^^^^^

.. java:method:: public MutationOperator<S> getMutation()
   :outertype: EvolutionStrategyBuilder

setLambda
^^^^^^^^^

.. java:method:: public EvolutionStrategyBuilder<S> setLambda(int lambda)
   :outertype: EvolutionStrategyBuilder

setMaxEvaluations
^^^^^^^^^^^^^^^^^

.. java:method:: public EvolutionStrategyBuilder<S> setMaxEvaluations(int maxEvaluations)
   :outertype: EvolutionStrategyBuilder

setMu
^^^^^

.. java:method:: public EvolutionStrategyBuilder<S> setMu(int mu)
   :outertype: EvolutionStrategyBuilder

