.. java:import:: org.uma.jmetal.algorithm.multiobjective.espea.util ScalarizationWrapper.ScalarizationType

.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util SolutionListUtils

.. java:import:: org.uma.jmetal.util.archive.impl AbstractBoundedArchive

.. java:import:: org.uma.jmetal.util.comparator FitnessComparator

.. java:import:: org.uma.jmetal.util.front.util FrontNormalizer

.. java:import:: org.uma.jmetal.util.solutionattribute.impl Fitness

.. java:import:: java.util Collections

.. java:import:: java.util Comparator

EnergyArchive.ReplacementStrategy
=================================

.. java:package:: org.uma.jmetal.algorithm.multiobjective.espea.util
   :noindex:

.. java:type:: public static enum ReplacementStrategy
   :outertype: EnergyArchive

   The replacement strategy defines the rule by which an existing archive member is replaced by a new solution. Computational studies have revealed that \ :java:ref:`BEST_FEASIBLE_POSITION`\  is inferior to \ :java:ref:`LARGEST_DIFFERENCE`\  and \ :java:ref:`WORST_IN_ARCHIVE`\ . No significant performance difference could be founnd between \ :java:ref:`LARGEST_DIFFERENCE`\  and \ :java:ref:`WORST_IN_ARCHIVE`\ . See "Obtaining Optimal Pareto Front Appxoimations" by Braun et al. and "Scalarized Preferences in Multi-objective Optimizaiton" by Braun for details.

   :author: marlon.braun

Enum Constants
--------------
BEST_FEASIBLE_POSITION
^^^^^^^^^^^^^^^^^^^^^^

.. java:field:: public static final EnergyArchive.ReplacementStrategy BEST_FEASIBLE_POSITION
   :outertype: EnergyArchive.ReplacementStrategy

   Inserts the new solution such that the energy it introduces into the archive is minimized.

LARGEST_DIFFERENCE
^^^^^^^^^^^^^^^^^^

.. java:field:: public static final EnergyArchive.ReplacementStrategy LARGEST_DIFFERENCE
   :outertype: EnergyArchive.ReplacementStrategy

   Maximizes the energy differences before and after replacement.

WORST_IN_ARCHIVE
^^^^^^^^^^^^^^^^

.. java:field:: public static final EnergyArchive.ReplacementStrategy WORST_IN_ARCHIVE
   :outertype: EnergyArchive.ReplacementStrategy

   Among all eligible archive members that can be replaced the one exhibiting the largest energy contribution is replaced.

