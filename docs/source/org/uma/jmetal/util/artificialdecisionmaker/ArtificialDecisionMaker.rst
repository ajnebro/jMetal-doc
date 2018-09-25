.. java:import:: org.uma.jmetal.algorithm Algorithm

.. java:import:: org.uma.jmetal.algorithm InteractiveAlgorithm

.. java:import:: org.uma.jmetal.problem Problem

.. java:import:: java.util ArrayList

.. java:import:: java.util List

ArtificialDecisionMaker
=======================

.. java:package:: org.uma.jmetal.util.artificialdecisionmaker
   :noindex:

.. java:type:: public abstract class ArtificialDecisionMaker<S, R> implements Algorithm<R>

Fields
------
algorithm
^^^^^^^^^

.. java:field:: protected InteractiveAlgorithm<S, R> algorithm
   :outertype: ArtificialDecisionMaker

indexOfRelevantObjectiveFunctions
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:field:: protected List<Integer> indexOfRelevantObjectiveFunctions
   :outertype: ArtificialDecisionMaker

paretoOptimalSolutions
^^^^^^^^^^^^^^^^^^^^^^

.. java:field:: protected List<S> paretoOptimalSolutions
   :outertype: ArtificialDecisionMaker

problem
^^^^^^^

.. java:field:: protected Problem<S> problem
   :outertype: ArtificialDecisionMaker

Constructors
------------
ArtificialDecisionMaker
^^^^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public ArtificialDecisionMaker(Problem<S> problem, InteractiveAlgorithm<S, R> algorithm)
   :outertype: ArtificialDecisionMaker

Methods
-------
calculateReferencePoints
^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: protected abstract List<Double> calculateReferencePoints(List<Integer> indexOfRelevantObjectiveFunctions, R front, List<S> paretoOptimalSolutions)
   :outertype: ArtificialDecisionMaker

generatePreferenceInformation
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: protected abstract List<Double> generatePreferenceInformation()
   :outertype: ArtificialDecisionMaker

getDescription
^^^^^^^^^^^^^^

.. java:method:: @Override public String getDescription()
   :outertype: ArtificialDecisionMaker

getDistances
^^^^^^^^^^^^

.. java:method:: public abstract List<Double> getDistances()
   :outertype: ArtificialDecisionMaker

getName
^^^^^^^

.. java:method:: @Override public String getName()
   :outertype: ArtificialDecisionMaker

getReferencePoints
^^^^^^^^^^^^^^^^^^

.. java:method:: public abstract List<Double> getReferencePoints()
   :outertype: ArtificialDecisionMaker

getResult
^^^^^^^^^

.. java:method:: @Override public R getResult()
   :outertype: ArtificialDecisionMaker

initProgress
^^^^^^^^^^^^

.. java:method:: protected abstract void initProgress()
   :outertype: ArtificialDecisionMaker

isStoppingConditionReached
^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: protected abstract boolean isStoppingConditionReached()
   :outertype: ArtificialDecisionMaker

relevantObjectiveFunctions
^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: protected abstract List<Integer> relevantObjectiveFunctions(R front)
   :outertype: ArtificialDecisionMaker

run
^^^

.. java:method:: @Override public void run()
   :outertype: ArtificialDecisionMaker

updateParetoOptimal
^^^^^^^^^^^^^^^^^^^

.. java:method:: protected abstract void updateParetoOptimal(R front, List<S> paretoOptimalSolutions)
   :outertype: ArtificialDecisionMaker

updateProgress
^^^^^^^^^^^^^^

.. java:method:: protected abstract void updateProgress()
   :outertype: ArtificialDecisionMaker

