.. java:import:: org.apache.commons.lang3.tuple ImmutablePair

.. java:import:: org.apache.commons.lang3.tuple Pair

.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util.pseudorandom JMetalRandom

.. java:import:: java.util ArrayList

.. java:import:: java.util Iterator

.. java:import:: java.util List

ReferencePoint
==============

.. java:package:: org.uma.jmetal.algorithm.multiobjective.nsgaiii.util
   :noindex:

.. java:type:: public class ReferencePoint<S extends Solution<?>>

   Created by ajnebro on 5/11/14. Modified by Juanjo on 13/11/14 This implementation is based on the code of Tsung-Che Chiang http://web.ntnu.edu.tw/~tcchiang/publications/nsga3cpp/nsga3cpp.htm

Fields
------
position
^^^^^^^^

.. java:field:: public List<Double> position
   :outertype: ReferencePoint

Constructors
------------
ReferencePoint
^^^^^^^^^^^^^^

.. java:constructor:: public ReferencePoint()
   :outertype: ReferencePoint

ReferencePoint
^^^^^^^^^^^^^^

.. java:constructor:: public ReferencePoint(int size)
   :outertype: ReferencePoint

   Constructor

ReferencePoint
^^^^^^^^^^^^^^

.. java:constructor:: public ReferencePoint(ReferencePoint<S> point)
   :outertype: ReferencePoint

Methods
-------
AddMember
^^^^^^^^^

.. java:method:: public void AddMember()
   :outertype: ReferencePoint

AddPotentialMember
^^^^^^^^^^^^^^^^^^

.. java:method:: public void AddPotentialMember(S member_ind, double distance)
   :outertype: ReferencePoint

FindClosestMember
^^^^^^^^^^^^^^^^^

.. java:method:: public S FindClosestMember()
   :outertype: ReferencePoint

HasPotentialMember
^^^^^^^^^^^^^^^^^^

.. java:method:: public boolean HasPotentialMember()
   :outertype: ReferencePoint

MemberSize
^^^^^^^^^^

.. java:method:: public int MemberSize()
   :outertype: ReferencePoint

RandomMember
^^^^^^^^^^^^

.. java:method:: public S RandomMember()
   :outertype: ReferencePoint

RemovePotentialMember
^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public void RemovePotentialMember(S solution)
   :outertype: ReferencePoint

clear
^^^^^

.. java:method:: public void clear()
   :outertype: ReferencePoint

generateReferencePoints
^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public void generateReferencePoints(List<ReferencePoint<S>> referencePoints, int numberOfObjectives, List<Integer> numberOfDivisions)
   :outertype: ReferencePoint

pos
^^^

.. java:method:: public List<Double> pos()
   :outertype: ReferencePoint

