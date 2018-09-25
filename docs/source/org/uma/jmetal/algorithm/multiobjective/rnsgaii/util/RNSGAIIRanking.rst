.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util.comparator ObjectiveComparator

.. java:import:: org.uma.jmetal.util.pseudorandom JMetalRandom

.. java:import:: org.uma.jmetal.util.solutionattribute Ranking

.. java:import:: org.uma.jmetal.util.solutionattribute.impl GenericSolutionAttribute

.. java:import:: org.uma.jmetal.util.solutionattribute.impl NumberOfViolatedConstraints

RNSGAIIRanking
==============

.. java:package:: org.uma.jmetal.algorithm.multiobjective.rnsgaii.util
   :noindex:

.. java:type:: public class RNSGAIIRanking<S extends Solution<?>> extends GenericSolutionAttribute<S, Integer> implements Ranking<S>

Constructors
------------
RNSGAIIRanking
^^^^^^^^^^^^^^

.. java:constructor:: public RNSGAIIRanking(PreferenceNSGAII<S> utilityFunctions, double epsilon, List<Double> interestPoint)
   :outertype: RNSGAIIRanking

Methods
-------
computeRanking
^^^^^^^^^^^^^^

.. java:method:: @Override public Ranking<S> computeRanking(List<S> population)
   :outertype: RNSGAIIRanking

getNumberOfSubfronts
^^^^^^^^^^^^^^^^^^^^

.. java:method:: public int getNumberOfSubfronts()
   :outertype: RNSGAIIRanking

getSubfront
^^^^^^^^^^^

.. java:method:: public List<S> getSubfront(int rank)
   :outertype: RNSGAIIRanking

