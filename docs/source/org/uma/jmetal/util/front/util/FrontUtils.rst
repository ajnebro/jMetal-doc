.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: org.uma.jmetal.util.front Front

.. java:import:: org.uma.jmetal.util.front.imp ArrayFront

.. java:import:: org.uma.jmetal.util.point Point

.. java:import:: org.uma.jmetal.util.point PointSolution

.. java:import:: org.uma.jmetal.util.point.util.distance EuclideanDistance

.. java:import:: org.uma.jmetal.util.point.util.distance PointDistance

.. java:import:: java.util ArrayList

.. java:import:: java.util List

FrontUtils
==========

.. java:package:: org.uma.jmetal.util.front.util
   :noindex:

.. java:type:: public class FrontUtils

   A Front is a list of points. This class includes utilities to work with \ :java:ref:`Front`\  objects.

   :author: Antonio J. Nebro

Methods
-------
convertFrontToArray
^^^^^^^^^^^^^^^^^^^

.. java:method:: public static double[][] convertFrontToArray(Front front)
   :outertype: FrontUtils

   Given a front, converts it to an array of double values

   :param front:
   :return: A front as double[][] array

convertFrontToSolutionList
^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public static List<PointSolution> convertFrontToSolutionList(Front front)
   :outertype: FrontUtils

   Given a front, converts it to a Solution set of PointSolutions

   :param front:
   :return: A front as a List

distanceToClosestPoint
^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public static double distanceToClosestPoint(Point point, Front front)
   :outertype: FrontUtils

   Gets the distance between a point and the nearest one in a given front. The Euclidean distance is assumed

   :param point: The point
   :param front: The front that contains the other points to calculate the distances
   :return: The minimum distance between the point and the front

distanceToClosestPoint
^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public static double distanceToClosestPoint(Point point, Front front, PointDistance distance)
   :outertype: FrontUtils

   Gets the distance between a point and the nearest one in a given front

   :param point: The point
   :param front: The front that contains the other points to calculate the distances
   :return: The minimum distance between the point and the front

distanceToNearestPoint
^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public static double distanceToNearestPoint(Point point, Front front)
   :outertype: FrontUtils

   Gets the distance between a point and the nearest one in a front. If a distance equals to 0 is found, that means that the point is in the front, so it is excluded

   :param point: The point
   :param front: The front that contains the other points to calculate the distances
   :return: The minimum distance between the point and the front

distanceToNearestPoint
^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public static double distanceToNearestPoint(Point point, Front front, PointDistance distance)
   :outertype: FrontUtils

   Gets the distance between a point and the nearest one in a front. If a distance equals to 0 is found, that means that the point is in the front, so it is excluded

   :param point: The point
   :param front: The front that contains the other points to calculate the distances
   :return: The minimum distance between the point and the front

getInvertedFront
^^^^^^^^^^^^^^^^

.. java:method:: public static Front getInvertedFront(Front front)
   :outertype: FrontUtils

   This method receives a normalized pareto front and return the inverted one. This method is for minimization problems

   :param front: The pareto front to inverse
   :return: The inverted pareto front

getMaximumValues
^^^^^^^^^^^^^^^^

.. java:method:: public static double[] getMaximumValues(Front front)
   :outertype: FrontUtils

   Gets the maximum values for each objectives in a front

   :param front: A front of objective values
   :return: double [] An array with the maximum values for each objective

getMinimumValues
^^^^^^^^^^^^^^^^

.. java:method:: public static double[] getMinimumValues(Front front)
   :outertype: FrontUtils

   Gets the minimum values for each objectives in a given front

   :param front: The front
   :return: double [] An array with the minimum value for each objective

