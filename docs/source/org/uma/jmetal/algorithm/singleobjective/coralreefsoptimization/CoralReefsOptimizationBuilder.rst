.. java:import:: org.uma.jmetal.operator CrossoverOperator

.. java:import:: org.uma.jmetal.operator MutationOperator

.. java:import:: org.uma.jmetal.operator SelectionOperator

.. java:import:: org.uma.jmetal.problem Problem

.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util AlgorithmBuilder

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: java.util Comparator

.. java:import:: java.util List

CoralReefsOptimizationBuilder
=============================

.. java:package:: org.uma.jmetal.algorithm.singleobjective.coralreefsoptimization
   :noindex:

.. java:type:: public class CoralReefsOptimizationBuilder<S extends Solution<?>> implements AlgorithmBuilder<CoralReefsOptimization<S>>

   :author: Inacio Medeiros

Constructors
------------
CoralReefsOptimizationBuilder
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public CoralReefsOptimizationBuilder(Problem<S> problem, SelectionOperator<List<S>, S> selectionOperator, CrossoverOperator<S> crossoverOperator, MutationOperator<S> mutationOperator)
   :outertype: CoralReefsOptimizationBuilder

   CoralReefsOptimizationBuilder constructor

Methods
-------
build
^^^^^

.. java:method:: @Override public CoralReefsOptimization<S> build()
   :outertype: CoralReefsOptimizationBuilder

getAttemptsToSettle
^^^^^^^^^^^^^^^^^^^

.. java:method:: public int getAttemptsToSettle()
   :outertype: CoralReefsOptimizationBuilder

getComparator
^^^^^^^^^^^^^

.. java:method:: public Comparator<S> getComparator()
   :outertype: CoralReefsOptimizationBuilder

getCrossoverOperator
^^^^^^^^^^^^^^^^^^^^

.. java:method:: public CrossoverOperator<S> getCrossoverOperator()
   :outertype: CoralReefsOptimizationBuilder

getFa
^^^^^

.. java:method:: public double getFa()
   :outertype: CoralReefsOptimizationBuilder

getFbr
^^^^^^

.. java:method:: public double getFbr()
   :outertype: CoralReefsOptimizationBuilder

getFbs
^^^^^^

.. java:method:: public double getFbs()
   :outertype: CoralReefsOptimizationBuilder

getFd
^^^^^

.. java:method:: public double getFd()
   :outertype: CoralReefsOptimizationBuilder

getM
^^^^

.. java:method:: public int getM()
   :outertype: CoralReefsOptimizationBuilder

getMaxEvaluations
^^^^^^^^^^^^^^^^^

.. java:method:: public int getMaxEvaluations()
   :outertype: CoralReefsOptimizationBuilder

getMutationOperator
^^^^^^^^^^^^^^^^^^^

.. java:method:: public MutationOperator<S> getMutationOperator()
   :outertype: CoralReefsOptimizationBuilder

getN
^^^^

.. java:method:: public int getN()
   :outertype: CoralReefsOptimizationBuilder

getPd
^^^^^

.. java:method:: public double getPd()
   :outertype: CoralReefsOptimizationBuilder

getProblem
^^^^^^^^^^

.. java:method:: public Problem<S> getProblem()
   :outertype: CoralReefsOptimizationBuilder

getRho
^^^^^^

.. java:method:: public double getRho()
   :outertype: CoralReefsOptimizationBuilder

getSelectionOperator
^^^^^^^^^^^^^^^^^^^^

.. java:method:: public SelectionOperator<List<S>, S> getSelectionOperator()
   :outertype: CoralReefsOptimizationBuilder

setAttemptsToSettle
^^^^^^^^^^^^^^^^^^^

.. java:method:: public CoralReefsOptimizationBuilder<S> setAttemptsToSettle(int attemptsToSettle)
   :outertype: CoralReefsOptimizationBuilder

setComparator
^^^^^^^^^^^^^

.. java:method:: public CoralReefsOptimizationBuilder<S> setComparator(Comparator<S> comparator)
   :outertype: CoralReefsOptimizationBuilder

setFa
^^^^^

.. java:method:: public CoralReefsOptimizationBuilder<S> setFa(double fa)
   :outertype: CoralReefsOptimizationBuilder

setFbr
^^^^^^

.. java:method:: public CoralReefsOptimizationBuilder<S> setFbr(double fbr)
   :outertype: CoralReefsOptimizationBuilder

setFbs
^^^^^^

.. java:method:: public CoralReefsOptimizationBuilder<S> setFbs(double fbs)
   :outertype: CoralReefsOptimizationBuilder

setFd
^^^^^

.. java:method:: public CoralReefsOptimizationBuilder<S> setFd(double fd)
   :outertype: CoralReefsOptimizationBuilder

setM
^^^^

.. java:method:: public CoralReefsOptimizationBuilder<S> setM(int m)
   :outertype: CoralReefsOptimizationBuilder

setMaxEvaluations
^^^^^^^^^^^^^^^^^

.. java:method:: public CoralReefsOptimizationBuilder<S> setMaxEvaluations(int maxEvaluations)
   :outertype: CoralReefsOptimizationBuilder

setN
^^^^

.. java:method:: public CoralReefsOptimizationBuilder<S> setN(int n)
   :outertype: CoralReefsOptimizationBuilder

setPd
^^^^^

.. java:method:: public CoralReefsOptimizationBuilder<S> setPd(double pd)
   :outertype: CoralReefsOptimizationBuilder

setRho
^^^^^^

.. java:method:: public CoralReefsOptimizationBuilder<S> setRho(double rho)
   :outertype: CoralReefsOptimizationBuilder

