.. java:import:: org.uma.jmetal.algorithm Algorithm

.. java:import:: org.uma.jmetal.operator CrossoverOperator

.. java:import:: org.uma.jmetal.operator MutationOperator

.. java:import:: org.uma.jmetal.operator SelectionOperator

.. java:import:: java.util ArrayList

.. java:import:: java.util Collections

.. java:import:: java.util Comparator

.. java:import:: java.util List

AbstractCoralReefsOptimization
==============================

.. java:package:: org.uma.jmetal.algorithm.impl
   :noindex:

.. java:type:: @SuppressWarnings public abstract class AbstractCoralReefsOptimization<S, R> implements Algorithm<R>

   Abstract class representing a Coral Reefs Optimization Algorithm Reference: S. Salcedo-Sanz, J. Del Ser, S. Gil-López, I. Landa-Torres and J. A. Portilla-Figueras, "The coral reefs optimization algorithm: an efficient meta-heuristic for solving hard optimization problems," 15th Applied Stochastic Models and Data Analysis International Conference, Mataró, Spain, June, 2013.

   :author: Inacio Medeiros

Fields
------
comparator
^^^^^^^^^^

.. java:field:: protected Comparator<S> comparator
   :outertype: AbstractCoralReefsOptimization

coordinates
^^^^^^^^^^^

.. java:field:: protected List<Coordinate> coordinates
   :outertype: AbstractCoralReefsOptimization

crossoverOperator
^^^^^^^^^^^^^^^^^

.. java:field:: protected CrossoverOperator<S> crossoverOperator
   :outertype: AbstractCoralReefsOptimization

mutationOperator
^^^^^^^^^^^^^^^^

.. java:field:: protected MutationOperator<S> mutationOperator
   :outertype: AbstractCoralReefsOptimization

population
^^^^^^^^^^

.. java:field:: protected List<S> population
   :outertype: AbstractCoralReefsOptimization

selectionOperator
^^^^^^^^^^^^^^^^^

.. java:field:: protected SelectionOperator<List<S>, S> selectionOperator
   :outertype: AbstractCoralReefsOptimization

Constructors
------------
AbstractCoralReefsOptimization
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public AbstractCoralReefsOptimization(Comparator<S> comparator, SelectionOperator<List<S>, S> selectionOperator, CrossoverOperator<S> crossoverOperator, MutationOperator<S> mutationOperator, int n, int m, double rho, double fbs, double fa, double pd, int attemptsToSettle)
   :outertype: AbstractCoralReefsOptimization

   Constructor

   :param comparator: Object for comparing two solutions
   :param selectionOperator: Selection Operator
   :param crossoverOperator: Crossover Operator
   :param mutationOperator: Mutation Operator
   :param n: width of Coral Reef Grid
   :param m: height of Coral Reef Grid
   :param rho: Percentage of occupied reef
   :param fbs: Percentage of broadcast spawners
   :param fa: Percentage of budders
   :param pd: Probability of depredation
   :param attemptsToSettle: number of attempts a larvae has to try to settle reef

Methods
-------
asexualReproduction
^^^^^^^^^^^^^^^^^^^

.. java:method:: protected abstract List<S> asexualReproduction(List<S> brooders)
   :outertype: AbstractCoralReefsOptimization

createInitialPopulation
^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: protected abstract List<S> createInitialPopulation()
   :outertype: AbstractCoralReefsOptimization

depredation
^^^^^^^^^^^

.. java:method:: protected abstract List<S> depredation(List<S> population, List<Coordinate> coordinates)
   :outertype: AbstractCoralReefsOptimization

evaluatePopulation
^^^^^^^^^^^^^^^^^^

.. java:method:: protected abstract List<S> evaluatePopulation(List<S> population)
   :outertype: AbstractCoralReefsOptimization

generateCoordinates
^^^^^^^^^^^^^^^^^^^

.. java:method:: protected abstract List<Coordinate> generateCoordinates()
   :outertype: AbstractCoralReefsOptimization

getAttemptsToSettle
^^^^^^^^^^^^^^^^^^^

.. java:method:: public int getAttemptsToSettle()
   :outertype: AbstractCoralReefsOptimization

getCoordinates
^^^^^^^^^^^^^^

.. java:method:: public List<Coordinate> getCoordinates()
   :outertype: AbstractCoralReefsOptimization

getFa
^^^^^

.. java:method:: public double getFa()
   :outertype: AbstractCoralReefsOptimization

getFbr
^^^^^^

.. java:method:: public double getFbr()
   :outertype: AbstractCoralReefsOptimization

getFbs
^^^^^^

.. java:method:: public double getFbs()
   :outertype: AbstractCoralReefsOptimization

getFd
^^^^^

.. java:method:: public double getFd()
   :outertype: AbstractCoralReefsOptimization

getM
^^^^

.. java:method:: public int getM()
   :outertype: AbstractCoralReefsOptimization

getN
^^^^

.. java:method:: public int getN()
   :outertype: AbstractCoralReefsOptimization

getPd
^^^^^

.. java:method:: public double getPd()
   :outertype: AbstractCoralReefsOptimization

getPopulation
^^^^^^^^^^^^^

.. java:method:: public List<S> getPopulation()
   :outertype: AbstractCoralReefsOptimization

getPopulationSize
^^^^^^^^^^^^^^^^^

.. java:method:: public int getPopulationSize()
   :outertype: AbstractCoralReefsOptimization

getResult
^^^^^^^^^

.. java:method:: @Override public abstract R getResult()
   :outertype: AbstractCoralReefsOptimization

getRho
^^^^^^

.. java:method:: public double getRho()
   :outertype: AbstractCoralReefsOptimization

initProgress
^^^^^^^^^^^^

.. java:method:: protected abstract void initProgress()
   :outertype: AbstractCoralReefsOptimization

isStoppingConditionReached
^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: protected abstract boolean isStoppingConditionReached()
   :outertype: AbstractCoralReefsOptimization

larvaeSettlementPhase
^^^^^^^^^^^^^^^^^^^^^

.. java:method:: protected abstract List<S> larvaeSettlementPhase(List<S> larvae, List<S> population, List<Coordinate> coordinates)
   :outertype: AbstractCoralReefsOptimization

run
^^^

.. java:method:: @Override public void run()
   :outertype: AbstractCoralReefsOptimization

selectBroadcastSpawners
^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: protected abstract List<S> selectBroadcastSpawners(List<S> population)
   :outertype: AbstractCoralReefsOptimization

setCoordinates
^^^^^^^^^^^^^^

.. java:method:: public void setCoordinates(List<Coordinate> coordinates)
   :outertype: AbstractCoralReefsOptimization

setPopulation
^^^^^^^^^^^^^

.. java:method:: public void setPopulation(List<S> population)
   :outertype: AbstractCoralReefsOptimization

sexualReproduction
^^^^^^^^^^^^^^^^^^

.. java:method:: protected abstract List<S> sexualReproduction(List<S> broadcastSpawners)
   :outertype: AbstractCoralReefsOptimization

updateProgress
^^^^^^^^^^^^^^

.. java:method:: protected abstract void updateProgress()
   :outertype: AbstractCoralReefsOptimization

