.. java:import:: org.uma.jmetal.algorithm InteractiveAlgorithm

.. java:import:: org.uma.jmetal.problem Problem

.. java:import:: org.uma.jmetal.problem.impl AbstractDoubleProblem

.. java:import:: org.uma.jmetal.problem.impl AbstractIntegerDoubleProblem

.. java:import:: org.uma.jmetal.problem.impl AbstractIntegerProblem

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util.artificialdecisionmaker ArtificialDecisionMaker

.. java:import:: org.uma.jmetal.util.artificialdecisionmaker DecisionTreeEstimator

.. java:import:: org.uma.jmetal.util.comparator ObjectiveComparator

.. java:import:: org.uma.jmetal.util.distance.impl EuclideanDistanceBetweenSolutionsInObjectiveSpace

.. java:import:: org.uma.jmetal.util.pseudorandom JMetalRandom

ArtificialDecisionMakerDecisionTree
===================================

.. java:package:: org.uma.jmetal.util.artificialdecisionmaker.impl
   :noindex:

.. java:type:: public class ArtificialDecisionMakerDecisionTree<S extends Solution<?>> extends ArtificialDecisionMaker<S, List<S>>

   Class implementing the Towards automatic testing of reference point based interactive methods described in: Ojalehto, V., Podkopaev, D., & Miettinen, K. (2016, September). Towards automatic testing of reference point based interactive methods. In International Conference on Parallel Problem Solving from Nature (pp. 483-492). Springer, Cham.

   :author: Cristobal Barba

Fields
------
allReferencePoints
^^^^^^^^^^^^^^^^^^

.. java:field:: protected List<Double> allReferencePoints
   :outertype: ArtificialDecisionMakerDecisionTree

asp
^^^

.. java:field:: protected List<Double> asp
   :outertype: ArtificialDecisionMakerDecisionTree

considerationProbability
^^^^^^^^^^^^^^^^^^^^^^^^

.. java:field:: protected double considerationProbability
   :outertype: ArtificialDecisionMakerDecisionTree

currentReferencePoint
^^^^^^^^^^^^^^^^^^^^^

.. java:field:: protected List<Double> currentReferencePoint
   :outertype: ArtificialDecisionMakerDecisionTree

distances
^^^^^^^^^

.. java:field:: protected List<Double> distances
   :outertype: ArtificialDecisionMakerDecisionTree

evaluations
^^^^^^^^^^^

.. java:field:: protected int evaluations
   :outertype: ArtificialDecisionMakerDecisionTree

idealOjectiveVector
^^^^^^^^^^^^^^^^^^^

.. java:field:: protected List<Double> idealOjectiveVector
   :outertype: ArtificialDecisionMakerDecisionTree

maxEvaluations
^^^^^^^^^^^^^^

.. java:field:: protected int maxEvaluations
   :outertype: ArtificialDecisionMakerDecisionTree

nadirObjectiveVector
^^^^^^^^^^^^^^^^^^^^

.. java:field:: protected List<Double> nadirObjectiveVector
   :outertype: ArtificialDecisionMakerDecisionTree

numberOfObjectives
^^^^^^^^^^^^^^^^^^

.. java:field:: protected int numberOfObjectives
   :outertype: ArtificialDecisionMakerDecisionTree

random
^^^^^^

.. java:field:: protected JMetalRandom random
   :outertype: ArtificialDecisionMakerDecisionTree

rankingCoeficient
^^^^^^^^^^^^^^^^^

.. java:field:: protected List<Double> rankingCoeficient
   :outertype: ArtificialDecisionMakerDecisionTree

tolerance
^^^^^^^^^

.. java:field:: protected double tolerance
   :outertype: ArtificialDecisionMakerDecisionTree

varyingProbability
^^^^^^^^^^^^^^^^^^

.. java:field:: protected double varyingProbability
   :outertype: ArtificialDecisionMakerDecisionTree

Constructors
------------
ArtificialDecisionMakerDecisionTree
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public ArtificialDecisionMakerDecisionTree(Problem<S> problem, InteractiveAlgorithm<S, List<S>> algorithm, double considerationProbability, double tolerance, int maxEvaluations, List<Double> rankingCoeficient, List<Double> asp)
   :outertype: ArtificialDecisionMakerDecisionTree

Methods
-------
calculateReferencePoints
^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override protected List<Double> calculateReferencePoints(List<Integer> indexOfRelevantObjectiveFunctions, List<S> front, List<S> paretoOptimalSolutions)
   :outertype: ArtificialDecisionMakerDecisionTree

generatePreferenceInformation
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override protected List<Double> generatePreferenceInformation()
   :outertype: ArtificialDecisionMakerDecisionTree

getDistances
^^^^^^^^^^^^

.. java:method:: @Override public List<Double> getDistances()
   :outertype: ArtificialDecisionMakerDecisionTree

getReferencePoints
^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public List<Double> getReferencePoints()
   :outertype: ArtificialDecisionMakerDecisionTree

initProgress
^^^^^^^^^^^^

.. java:method:: @Override protected void initProgress()
   :outertype: ArtificialDecisionMakerDecisionTree

isStoppingConditionReached
^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override protected boolean isStoppingConditionReached()
   :outertype: ArtificialDecisionMakerDecisionTree

relevantObjectiveFunctions
^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override protected List<Integer> relevantObjectiveFunctions(List<S> front)
   :outertype: ArtificialDecisionMakerDecisionTree

updateParetoOptimal
^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override protected void updateParetoOptimal(List<S> front, List<S> paretoOptimalSolutions)
   :outertype: ArtificialDecisionMakerDecisionTree

updateProgress
^^^^^^^^^^^^^^

.. java:method:: @Override protected void updateProgress()
   :outertype: ArtificialDecisionMakerDecisionTree

