.. java:import:: org.uma.jmetal.algorithm Algorithm

.. java:import:: org.uma.jmetal.operator CrossoverOperator

.. java:import:: org.uma.jmetal.operator MutationOperator

.. java:import:: org.uma.jmetal.operator SelectionOperator

.. java:import:: org.uma.jmetal.problem Problem

.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util SolutionListUtils

.. java:import:: org.uma.jmetal.util.comparator DominanceComparator

.. java:import:: org.uma.jmetal.util.solutionattribute.impl Fitness

.. java:import:: java.util ArrayList

.. java:import:: java.util List

IBEA
====

.. java:package:: org.uma.jmetal.algorithm.multiobjective.ibea
   :noindex:

.. java:type:: @SuppressWarnings public class IBEA<S extends Solution<?>> implements Algorithm<List<S>>

   This class implements the IBEA algorithm

Fields
------
TOURNAMENTS_ROUNDS
^^^^^^^^^^^^^^^^^^

.. java:field:: public static final int TOURNAMENTS_ROUNDS
   :outertype: IBEA

archive
^^^^^^^

.. java:field:: protected List<S> archive
   :outertype: IBEA

archiveSize
^^^^^^^^^^^

.. java:field:: protected int archiveSize
   :outertype: IBEA

crossoverOperator
^^^^^^^^^^^^^^^^^

.. java:field:: protected CrossoverOperator<S> crossoverOperator
   :outertype: IBEA

indicatorValues
^^^^^^^^^^^^^^^

.. java:field:: protected List<List<Double>> indicatorValues
   :outertype: IBEA

maxEvaluations
^^^^^^^^^^^^^^

.. java:field:: protected int maxEvaluations
   :outertype: IBEA

maxIndicatorValue
^^^^^^^^^^^^^^^^^

.. java:field:: protected double maxIndicatorValue
   :outertype: IBEA

mutationOperator
^^^^^^^^^^^^^^^^

.. java:field:: protected MutationOperator<S> mutationOperator
   :outertype: IBEA

populationSize
^^^^^^^^^^^^^^

.. java:field:: protected int populationSize
   :outertype: IBEA

problem
^^^^^^^

.. java:field:: protected Problem<S> problem
   :outertype: IBEA

selectionOperator
^^^^^^^^^^^^^^^^^

.. java:field:: protected SelectionOperator<List<S>, S> selectionOperator
   :outertype: IBEA

solutionFitness
^^^^^^^^^^^^^^^

.. java:field:: protected Fitness<S> solutionFitness
   :outertype: IBEA

Constructors
------------
IBEA
^^^^

.. java:constructor:: public IBEA(Problem<S> problem, int populationSize, int archiveSize, int maxEvaluations, SelectionOperator<List<S>, S> selectionOperator, CrossoverOperator<S> crossoverOperator, MutationOperator<S> mutationOperator)
   :outertype: IBEA

   Constructor

Methods
-------
calculateFitness
^^^^^^^^^^^^^^^^

.. java:method:: public void calculateFitness(List<S> solutionSet)
   :outertype: IBEA

   Calculate the fitness for the entire population.

calculateHypervolumeIndicator
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method::  double calculateHypervolumeIndicator(Solution<?> solutionA, Solution<?> solutionB, int d, double[] maximumValues, double[] minimumValues)
   :outertype: IBEA

   Calculates the hypervolume of that portion of the objective space that is dominated by individual a but not by individual b

computeIndicatorValuesHD
^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public void computeIndicatorValuesHD(List<S> solutionSet, double[] maximumValues, double[] minimumValues)
   :outertype: IBEA

   This structure stores the indicator values of each pair of elements

fitness
^^^^^^^

.. java:method:: public void fitness(List<S> solutionSet, int pos)
   :outertype: IBEA

   Calculate the fitness for the individual at position pos

getDescription
^^^^^^^^^^^^^^

.. java:method:: @Override public String getDescription()
   :outertype: IBEA

getName
^^^^^^^

.. java:method:: @Override public String getName()
   :outertype: IBEA

getResult
^^^^^^^^^

.. java:method:: @Override public List<S> getResult()
   :outertype: IBEA

removeWorst
^^^^^^^^^^^

.. java:method:: public void removeWorst(List<S> solutionSet)
   :outertype: IBEA

   Update the fitness before removing an individual

run
^^^

.. java:method:: @Override public void run()
   :outertype: IBEA

   Execute() method

