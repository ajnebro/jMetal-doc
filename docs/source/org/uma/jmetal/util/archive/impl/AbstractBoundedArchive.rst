.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util.archive Archive

.. java:import:: org.uma.jmetal.util.archive BoundedArchive

.. java:import:: java.util List

AbstractBoundedArchive
======================

.. java:package:: org.uma.jmetal.util.archive.impl
   :noindex:

.. java:type:: @SuppressWarnings public abstract class AbstractBoundedArchive<S extends Solution<?>> implements BoundedArchive<S>

   :author: Antonio J. Nebro
   :param <S>:

Fields
------
archive
^^^^^^^

.. java:field:: protected NonDominatedSolutionListArchive<S> archive
   :outertype: AbstractBoundedArchive

maxSize
^^^^^^^

.. java:field:: protected int maxSize
   :outertype: AbstractBoundedArchive

Constructors
------------
AbstractBoundedArchive
^^^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public AbstractBoundedArchive(int maxSize)
   :outertype: AbstractBoundedArchive

Methods
-------
add
^^^

.. java:method:: @Override public boolean add(S solution)
   :outertype: AbstractBoundedArchive

get
^^^

.. java:method:: @Override public S get(int index)
   :outertype: AbstractBoundedArchive

getMaxSize
^^^^^^^^^^

.. java:method:: @Override public int getMaxSize()
   :outertype: AbstractBoundedArchive

getSolutionList
^^^^^^^^^^^^^^^

.. java:method:: @Override public List<S> getSolutionList()
   :outertype: AbstractBoundedArchive

join
^^^^

.. java:method:: public Archive<S> join(Archive<S> archive)
   :outertype: AbstractBoundedArchive

prune
^^^^^

.. java:method:: public abstract void prune()
   :outertype: AbstractBoundedArchive

size
^^^^

.. java:method:: @Override public int size()
   :outertype: AbstractBoundedArchive

