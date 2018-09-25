.. java:import:: org.uma.jmetal.algorithm Algorithm

.. java:import:: org.uma.jmetal.operator CrossoverOperator

.. java:import:: org.uma.jmetal.operator MutationOperator

.. java:import:: org.uma.jmetal.operator SelectionOperator

.. java:import:: java.util ArrayList

.. java:import:: java.util Collections

.. java:import:: java.util Comparator

.. java:import:: java.util List

AbstractCoralReefsOptimization.Coordinate
=========================================

.. java:package:: org.uma.jmetal.algorithm.impl
   :noindex:

.. java:type:: public static class Coordinate implements Comparable<Coordinate>
   :outertype: AbstractCoralReefsOptimization

   Represents a Coordinate in Coral Reef Grid

   :author: inacio-medeiros

Constructors
------------
Coordinate
^^^^^^^^^^

.. java:constructor:: public Coordinate(int x, int y)
   :outertype: AbstractCoralReefsOptimization.Coordinate

   Constructor

   :param x: Coordinate's x-position
   :param y: Coordinate's y-position

Methods
-------
compareTo
^^^^^^^^^

.. java:method:: @Override public int compareTo(Coordinate arg0)
   :outertype: AbstractCoralReefsOptimization.Coordinate

equals
^^^^^^

.. java:method:: @Override public boolean equals(Object obj)
   :outertype: AbstractCoralReefsOptimization.Coordinate

getX
^^^^

.. java:method:: public int getX()
   :outertype: AbstractCoralReefsOptimization.Coordinate

   Retrieves Coordinate's x-position

   :return: Coordinate's x-position

getY
^^^^

.. java:method:: public int getY()
   :outertype: AbstractCoralReefsOptimization.Coordinate

   Retrieves Coordinate's y-position

   :return: Coordinate's y-position

setX
^^^^

.. java:method:: public void setX(int x)
   :outertype: AbstractCoralReefsOptimization.Coordinate

   Sets Coordinate's x-position to a new value

   :param x: new value for Coordinate's x-position

setY
^^^^

.. java:method:: public void setY(int y)
   :outertype: AbstractCoralReefsOptimization.Coordinate

   Sets Coordinate's y-position to a new value

   :param x: new value for Coordinate's y-position

