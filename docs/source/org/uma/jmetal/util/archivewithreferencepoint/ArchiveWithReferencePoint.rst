.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util SolutionListUtils

.. java:import:: org.uma.jmetal.util.archive.impl AbstractBoundedArchive

.. java:import:: org.uma.jmetal.util.pseudorandom JMetalRandom

.. java:import:: java.util Comparator

.. java:import:: java.util List

ArchiveWithReferencePoint
=========================

.. java:package:: org.uma.jmetal.util.archivewithreferencepoint
   :noindex:

.. java:type:: public abstract class ArchiveWithReferencePoint<S extends Solution<?>> extends AbstractBoundedArchive<S>

   This class defines a bounded archive that has associated a reference point as described in the paper "Extending the Speed-constrained Multi-Objective PSO (SMPSO) With Reference Point Based Preference Articulation Accepted in PPSN 2018.

   :param <S>:

Fields
------
comparator
^^^^^^^^^^

.. java:field:: protected Comparator<S> comparator
   :outertype: ArchiveWithReferencePoint

referencePoint
^^^^^^^^^^^^^^

.. java:field:: protected List<Double> referencePoint
   :outertype: ArchiveWithReferencePoint

referencePointSolution
^^^^^^^^^^^^^^^^^^^^^^

.. java:field:: protected S referencePointSolution
   :outertype: ArchiveWithReferencePoint

Constructors
------------
ArchiveWithReferencePoint
^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public ArchiveWithReferencePoint(int maxSize, List<Double> referencePoint, Comparator<S> comparator)
   :outertype: ArchiveWithReferencePoint

Methods
-------
add
^^^

.. java:method:: @Override public synchronized boolean add(S solution)
   :outertype: ArchiveWithReferencePoint

changeReferencePoint
^^^^^^^^^^^^^^^^^^^^

.. java:method:: public synchronized void changeReferencePoint(List<Double> newReferencePoint)
   :outertype: ArchiveWithReferencePoint

prune
^^^^^

.. java:method:: @Override public synchronized void prune()
   :outertype: ArchiveWithReferencePoint

