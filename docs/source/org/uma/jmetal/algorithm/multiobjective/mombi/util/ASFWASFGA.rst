.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: java.util ArrayList

.. java:import:: java.util List

ASFWASFGA
=========

.. java:package:: org.uma.jmetal.algorithm.multiobjective.mombi.util
   :noindex:

.. java:type:: @SuppressWarnings public class ASFWASFGA<S extends Solution<?>> extends AbstractUtilityFunctionsSet<S>

   :author: Juan J. Durillo Modified by Antonio J. Nebro
   :param <S>:

Constructors
------------
ASFWASFGA
^^^^^^^^^

.. java:constructor:: public ASFWASFGA(double[][] weights, List<Double> interestPoint)
   :outertype: ASFWASFGA

ASFWASFGA
^^^^^^^^^

.. java:constructor:: public ASFWASFGA(double[][] weights)
   :outertype: ASFWASFGA

ASFWASFGA
^^^^^^^^^

.. java:constructor:: public ASFWASFGA(String file_path, List<Double> interestPoint)
   :outertype: ASFWASFGA

ASFWASFGA
^^^^^^^^^

.. java:constructor:: public ASFWASFGA(String file_path)
   :outertype: ASFWASFGA

Methods
-------
evaluate
^^^^^^^^

.. java:method:: @Override public Double evaluate(S solution, int vector)
   :outertype: ASFWASFGA

setNadir
^^^^^^^^

.. java:method:: public void setNadir(List<Double> nadir)
   :outertype: ASFWASFGA

setUtopia
^^^^^^^^^

.. java:method:: public void setUtopia(List<Double> utopia)
   :outertype: ASFWASFGA

updatePointOfInterest
^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public void updatePointOfInterest(List<Double> newInterestPoint)
   :outertype: ASFWASFGA

