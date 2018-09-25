.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: java.util Comparator

AchievementScalarizationComparator
==================================

.. java:package:: org.uma.jmetal.algorithm.multiobjective.espea.util
   :noindex:

.. java:type:: public class AchievementScalarizationComparator<S extends Solution<?>> implements Comparator<S>

   Compares solutions based on their achievement scalarization value (ASV). The ASV is always defined for a specific objective k. A solution x dominates solution y w.r.t. to their ASV, if the maximum of all objectives without k is smaller for x compared to y. If both maxima are the same, solutions are compared w.r.t. to objective k. Achievement scalarization values can be used for identifying extreme points.

   :author: marlon.braun
   :param <S>: The solution type.

Constructors
------------
AchievementScalarizationComparator
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public AchievementScalarizationComparator(int objective)
   :outertype: AchievementScalarizationComparator

   The achievement scalarization comparator requires an objective for which it is defined.

   :param objective: The objective for which achievement scalarizationv alues are computed.

Methods
-------
compare
^^^^^^^

.. java:method:: @Override public int compare(S s1, S s2)
   :outertype: AchievementScalarizationComparator

