.. java:import:: org.uma.jmetal.operator MutationOperator

.. java:import:: org.uma.jmetal.problem DoubleProblem

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.solution.util RepairDoubleSolution

.. java:import:: org.uma.jmetal.solution.util RepairDoubleSolutionAtBounds

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: org.uma.jmetal.util.pseudorandom JMetalRandom

CDGMutation
===========

.. java:package:: org.uma.jmetal.operator.impl.mutation
   :noindex:

.. java:type:: @SuppressWarnings public class CDGMutation implements MutationOperator<DoubleSolution>

   This class implements a polynomial mutation operator The implementation is based on the NSGA-II code available in http://www.iitk.ac.in/kangal/codes.shtml If the lower and upper bounds of a variable are the same, no mutation is carried out and the bound value is returned.

   :author: Feng Zhang

Constructors
------------
CDGMutation
^^^^^^^^^^^

.. java:constructor:: public CDGMutation()
   :outertype: CDGMutation

   Constructor

CDGMutation
^^^^^^^^^^^

.. java:constructor:: public CDGMutation(DoubleProblem problem, double delta)
   :outertype: CDGMutation

   Constructor

CDGMutation
^^^^^^^^^^^

.. java:constructor:: public CDGMutation(double mutationProbability, double delta)
   :outertype: CDGMutation

   Constructor

CDGMutation
^^^^^^^^^^^

.. java:constructor:: public CDGMutation(double mutationProbability, double delta, RepairDoubleSolution solutionRepair)
   :outertype: CDGMutation

   Constructor

Methods
-------
execute
^^^^^^^

.. java:method:: @Override public DoubleSolution execute(DoubleSolution solution) throws JMetalException
   :outertype: CDGMutation

   Execute() method

getDelta
^^^^^^^^

.. java:method:: public double getDelta()
   :outertype: CDGMutation

getMutationProbability
^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public double getMutationProbability()
   :outertype: CDGMutation

setDelta
^^^^^^^^

.. java:method:: public void setDelta(double delta)
   :outertype: CDGMutation

setMutationProbability
^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public void setMutationProbability(double probability)
   :outertype: CDGMutation

