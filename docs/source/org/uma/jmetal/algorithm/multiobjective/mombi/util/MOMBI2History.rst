.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: java.io Serializable

.. java:import:: java.util ArrayList

.. java:import:: java.util LinkedList

.. java:import:: java.util List

MOMBI2History
=============

.. java:package:: org.uma.jmetal.algorithm.multiobjective.mombi.util
   :noindex:

.. java:type:: @SuppressWarnings public class MOMBI2History<T extends Solution<?>> implements Serializable

   Created by ajnebro on 10/9/15.

Fields
------
MAX_LENGHT
^^^^^^^^^^

.. java:field:: public static final int MAX_LENGHT
   :outertype: MOMBI2History

Constructors
------------
MOMBI2History
^^^^^^^^^^^^^

.. java:constructor:: public MOMBI2History(int numberOfObjectives)
   :outertype: MOMBI2History

Methods
-------
add
^^^

.. java:method:: public void add(List<Double> maxs)
   :outertype: MOMBI2History

   Adds a new vector of maxs values to the history. The method ensures that only the newest MAX_LENGTH vectors will be kept in the history

   :param maxs:

decreaseMark
^^^^^^^^^^^^

.. java:method:: public void decreaseMark(int index)
   :outertype: MOMBI2History

getMaxObjective
^^^^^^^^^^^^^^^

.. java:method:: public Double getMaxObjective(int index)
   :outertype: MOMBI2History

isUnMarked
^^^^^^^^^^

.. java:method:: public boolean isUnMarked(int index)
   :outertype: MOMBI2History

mark
^^^^

.. java:method:: public void mark(int index)
   :outertype: MOMBI2History

mean
^^^^

.. java:method:: public List<Double> mean()
   :outertype: MOMBI2History

   Returns the mean of the values contained in the history

std
^^^

.. java:method:: public List<Double> std(List<Double> mean)
   :outertype: MOMBI2History

   Return the std of the values contained in the history

variance
^^^^^^^^

.. java:method:: public List<Double> variance(List<Double> mean)
   :outertype: MOMBI2History

   Returns the variance of the values contained in the history

