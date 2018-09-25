.. java:import:: org.uma.jmetal.operator CrossoverOperator

.. java:import:: org.uma.jmetal.operator LocalSearchOperator

.. java:import:: org.uma.jmetal.operator MutationOperator

.. java:import:: org.uma.jmetal.operator.impl.crossover SBXCrossover

.. java:import:: org.uma.jmetal.operator.impl.localsearch ArchiveMutationLocalSearch

.. java:import:: org.uma.jmetal.operator.impl.mutation PolynomialMutation

.. java:import:: org.uma.jmetal.problem DoubleProblem

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.util AlgorithmBuilder

.. java:import:: org.uma.jmetal.util.archive Archive

.. java:import:: org.uma.jmetal.util.archive.impl CrowdingDistanceArchive

ABYSSBuilder
============

.. java:package:: org.uma.jmetal.algorithm.multiobjective.abyss
   :noindex:

.. java:type:: public class ABYSSBuilder implements AlgorithmBuilder<ABYSS>

   :author: Cristobal Barba

Fields
------
improvementOperator
^^^^^^^^^^^^^^^^^^^

.. java:field:: protected LocalSearchOperator<DoubleSolution> improvementOperator
   :outertype: ABYSSBuilder

Constructors
------------
ABYSSBuilder
^^^^^^^^^^^^

.. java:constructor:: public ABYSSBuilder(DoubleProblem problem, Archive<DoubleSolution> archive)
   :outertype: ABYSSBuilder

Methods
-------
build
^^^^^

.. java:method:: @Override public ABYSS build()
   :outertype: ABYSSBuilder

getArchiveSize
^^^^^^^^^^^^^^

.. java:method:: public int getArchiveSize()
   :outertype: ABYSSBuilder

getCrossoverOperator
^^^^^^^^^^^^^^^^^^^^

.. java:method:: public CrossoverOperator<DoubleSolution> getCrossoverOperator()
   :outertype: ABYSSBuilder

getImprovementOperator
^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public LocalSearchOperator<DoubleSolution> getImprovementOperator()
   :outertype: ABYSSBuilder

getMaxEvaluations
^^^^^^^^^^^^^^^^^

.. java:method:: public int getMaxEvaluations()
   :outertype: ABYSSBuilder

getMutationOperator
^^^^^^^^^^^^^^^^^^^

.. java:method:: public MutationOperator<DoubleSolution> getMutationOperator()
   :outertype: ABYSSBuilder

getNumberOfSubranges
^^^^^^^^^^^^^^^^^^^^

.. java:method:: public int getNumberOfSubranges()
   :outertype: ABYSSBuilder

getPopulationSize
^^^^^^^^^^^^^^^^^

.. java:method:: public int getPopulationSize()
   :outertype: ABYSSBuilder

getRefSet1Size
^^^^^^^^^^^^^^

.. java:method:: public int getRefSet1Size()
   :outertype: ABYSSBuilder

getRefSet2Size
^^^^^^^^^^^^^^

.. java:method:: public int getRefSet2Size()
   :outertype: ABYSSBuilder

setArchiveSize
^^^^^^^^^^^^^^

.. java:method:: public ABYSSBuilder setArchiveSize(int archiveSize)
   :outertype: ABYSSBuilder

setCrossoverOperator
^^^^^^^^^^^^^^^^^^^^

.. java:method:: public ABYSSBuilder setCrossoverOperator(CrossoverOperator<DoubleSolution> crossoverOperator)
   :outertype: ABYSSBuilder

setImprovementOperator
^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public ABYSSBuilder setImprovementOperator(ArchiveMutationLocalSearch<DoubleSolution> improvementOperator)
   :outertype: ABYSSBuilder

setMaxEvaluations
^^^^^^^^^^^^^^^^^

.. java:method:: public ABYSSBuilder setMaxEvaluations(int maxEvaluations)
   :outertype: ABYSSBuilder

setMutationOperator
^^^^^^^^^^^^^^^^^^^

.. java:method:: public ABYSSBuilder setMutationOperator(MutationOperator<DoubleSolution> mutationOperator)
   :outertype: ABYSSBuilder

setNumberOfSubranges
^^^^^^^^^^^^^^^^^^^^

.. java:method:: public ABYSSBuilder setNumberOfSubranges(int numberOfSubranges)
   :outertype: ABYSSBuilder

setPopulationSize
^^^^^^^^^^^^^^^^^

.. java:method:: public ABYSSBuilder setPopulationSize(int populationSize)
   :outertype: ABYSSBuilder

setRefSet1Size
^^^^^^^^^^^^^^

.. java:method:: public ABYSSBuilder setRefSet1Size(int refSet1Size)
   :outertype: ABYSSBuilder

setRefSet2Size
^^^^^^^^^^^^^^

.. java:method:: public ABYSSBuilder setRefSet2Size(int refSet2Size)
   :outertype: ABYSSBuilder

