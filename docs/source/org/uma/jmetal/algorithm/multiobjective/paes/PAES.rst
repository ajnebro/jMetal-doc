.. java:import:: org.uma.jmetal.algorithm.impl AbstractEvolutionStrategy

.. java:import:: org.uma.jmetal.operator MutationOperator

.. java:import:: org.uma.jmetal.problem Problem

.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util.archive.impl AdaptiveGridArchive

.. java:import:: org.uma.jmetal.util.comparator DominanceComparator

.. java:import:: java.util ArrayList

.. java:import:: java.util Comparator

.. java:import:: java.util List

PAES
====

.. java:package:: org.uma.jmetal.algorithm.multiobjective.paes
   :noindex:

.. java:type:: @SuppressWarnings public class PAES<S extends Solution<?>> extends AbstractEvolutionStrategy<S, List<S>>

   :author: Antonio J. Nebro, Juan J. Durillo

Fields
------
archive
^^^^^^^

.. java:field:: protected AdaptiveGridArchive<S> archive
   :outertype: PAES

archiveSize
^^^^^^^^^^^

.. java:field:: protected int archiveSize
   :outertype: PAES

biSections
^^^^^^^^^^

.. java:field:: protected int biSections
   :outertype: PAES

comparator
^^^^^^^^^^

.. java:field:: protected Comparator<S> comparator
   :outertype: PAES

evaluations
^^^^^^^^^^^

.. java:field:: protected int evaluations
   :outertype: PAES

maxEvaluations
^^^^^^^^^^^^^^

.. java:field:: protected int maxEvaluations
   :outertype: PAES

Constructors
------------
PAES
^^^^

.. java:constructor:: public PAES(Problem<S> problem, int archiveSize, int maxEvaluations, int biSections, MutationOperator<S> mutationOperator)
   :outertype: PAES

   Constructor

Methods
-------
createInitialPopulation
^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override protected List<S> createInitialPopulation()
   :outertype: PAES

evaluatePopulation
^^^^^^^^^^^^^^^^^^

.. java:method:: @Override protected List<S> evaluatePopulation(List<S> population)
   :outertype: PAES

getArchiveSize
^^^^^^^^^^^^^^

.. java:method:: public int getArchiveSize()
   :outertype: PAES

getBiSections
^^^^^^^^^^^^^

.. java:method:: public int getBiSections()
   :outertype: PAES

getDescription
^^^^^^^^^^^^^^

.. java:method:: @Override public String getDescription()
   :outertype: PAES

getMaxEvaluations
^^^^^^^^^^^^^^^^^

.. java:method:: public int getMaxEvaluations()
   :outertype: PAES

getMutationOperator
^^^^^^^^^^^^^^^^^^^

.. java:method:: public MutationOperator<S> getMutationOperator()
   :outertype: PAES

getName
^^^^^^^

.. java:method:: @Override public String getName()
   :outertype: PAES

getResult
^^^^^^^^^

.. java:method:: @Override public List<S> getResult()
   :outertype: PAES

initProgress
^^^^^^^^^^^^

.. java:method:: @Override protected void initProgress()
   :outertype: PAES

isStoppingConditionReached
^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override protected boolean isStoppingConditionReached()
   :outertype: PAES

replacement
^^^^^^^^^^^

.. java:method:: @SuppressWarnings @Override protected List<S> replacement(List<S> population, List<S> offspringPopulation)
   :outertype: PAES

reproduction
^^^^^^^^^^^^

.. java:method:: @SuppressWarnings @Override protected List<S> reproduction(List<S> population)
   :outertype: PAES

selection
^^^^^^^^^

.. java:method:: @Override protected List<S> selection(List<S> population)
   :outertype: PAES

test
^^^^

.. java:method:: @SuppressWarnings public S test(S solution, S mutatedSolution, AdaptiveGridArchive<S> archive)
   :outertype: PAES

   Tests two solutions to determine which one becomes be the guide of PAES algorithm

   :param solution: The actual guide of PAES
   :param mutatedSolution: A candidate guide

updateProgress
^^^^^^^^^^^^^^

.. java:method:: @Override protected void updateProgress()
   :outertype: PAES

