.. java:import:: org.junit Test

.. java:import:: org.springframework.test.util ReflectionTestUtils

.. java:import:: org.uma.jmetal.solution IntegerSolution

.. java:import:: org.uma.jmetal.util.comparator DominanceComparator

NonDominatedSolutionListArchiveTest
===================================

.. java:package:: org.uma.jmetal.util.archive.impl
   :noindex:

.. java:type:: public class NonDominatedSolutionListArchiveTest

   :author: Antonio J. Nebro .

Methods
-------
shouldAddADominantSolutionInAnArchiveOfSize1DiscardTheExistingSolution
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldAddADominantSolutionInAnArchiveOfSize1DiscardTheExistingSolution()
   :outertype: NonDominatedSolutionListArchiveTest

shouldAddADominantSolutionInAnArchiveOfSize3DiscardTheRestOfSolutions
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldAddADominantSolutionInAnArchiveOfSize3DiscardTheRestOfSolutions()
   :outertype: NonDominatedSolutionListArchiveTest

shouldAddADominatedSolutionInAnArchiveOfSize1DiscardTheNewSolution
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldAddADominatedSolutionInAnArchiveOfSize1DiscardTheNewSolution()
   :outertype: NonDominatedSolutionListArchiveTest

shouldAddANonDominantSolutionInAnArchiveOfSize1IncorporateTheNewSolution
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldAddANonDominantSolutionInAnArchiveOfSize1IncorporateTheNewSolution()
   :outertype: NonDominatedSolutionListArchiveTest

shouldAddASolutionEqualsToOneAlreadyInTheArchiveDoNothing
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldAddASolutionEqualsToOneAlreadyInTheArchiveDoNothing()
   :outertype: NonDominatedSolutionListArchiveTest

shouldAddOnAnEmptyListHaveSizeOne
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldAddOnAnEmptyListHaveSizeOne()
   :outertype: NonDominatedSolutionListArchiveTest

shouldAddOnAnEmptyListInsertTheElement
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldAddOnAnEmptyListInsertTheElement()
   :outertype: NonDominatedSolutionListArchiveTest

shouldConstructorAssignThePassedComparator
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldConstructorAssignThePassedComparator()
   :outertype: NonDominatedSolutionListArchiveTest

shouldConstructorCreateAnEmptyArchive
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldConstructorCreateAnEmptyArchive()
   :outertype: NonDominatedSolutionListArchiveTest

shouldJoinAnEAnEmptyArchiveProduceAnArchiveWithTheSameSolutions
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldJoinAnEAnEmptyArchiveProduceAnArchiveWithTheSameSolutions()
   :outertype: NonDominatedSolutionListArchiveTest

shouldJoinTwoEmptyArchivesReturnAnEmptyArchive
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldJoinTwoEmptyArchivesReturnAnEmptyArchive()
   :outertype: NonDominatedSolutionListArchiveTest

shouldJoinWithAnEmptyArchivesRemainTheArchiveWithTheSameNumberOfSolutions
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: @Test public void shouldJoinWithAnEmptyArchivesRemainTheArchiveWithTheSameNumberOfSolutions()
   :outertype: NonDominatedSolutionListArchiveTest

