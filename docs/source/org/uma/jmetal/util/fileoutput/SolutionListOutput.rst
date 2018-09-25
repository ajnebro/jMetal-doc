.. java:import:: org.uma.jmetal.solution Solution

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: org.uma.jmetal.util.fileoutput.impl DefaultFileOutputContext

.. java:import:: java.io BufferedWriter

.. java:import:: java.io IOException

.. java:import:: java.util List

SolutionListOutput
==================

.. java:package:: org.uma.jmetal.util.fileoutput
   :noindex:

.. java:type:: public class SolutionListOutput

   :author: Antonio J. Nebro

Constructors
------------
SolutionListOutput
^^^^^^^^^^^^^^^^^^

.. java:constructor:: public SolutionListOutput(List<? extends Solution<?>> solutionList)
   :outertype: SolutionListOutput

Methods
-------
print
^^^^^

.. java:method:: public void print()
   :outertype: SolutionListOutput

printObjectivesToFile
^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public void printObjectivesToFile(FileOutputContext context, List<? extends Solution<?>> solutionList)
   :outertype: SolutionListOutput

printObjectivesToFile
^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public void printObjectivesToFile(FileOutputContext context, List<? extends Solution<?>> solutionList, List<Boolean> minimizeObjective)
   :outertype: SolutionListOutput

printObjectivesToFile
^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public void printObjectivesToFile(String fileName) throws IOException
   :outertype: SolutionListOutput

printObjectivesToFile
^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public void printObjectivesToFile(String fileName, List<Boolean> minimizeObjective) throws IOException
   :outertype: SolutionListOutput

printVariablesToFile
^^^^^^^^^^^^^^^^^^^^

.. java:method:: public void printVariablesToFile(FileOutputContext context, List<? extends Solution<?>> solutionList)
   :outertype: SolutionListOutput

printVariablesToFile
^^^^^^^^^^^^^^^^^^^^

.. java:method:: public void printVariablesToFile(String fileName) throws IOException
   :outertype: SolutionListOutput

setFunFileOutputContext
^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public SolutionListOutput setFunFileOutputContext(FileOutputContext fileContext)
   :outertype: SolutionListOutput

setObjectiveMinimizingObjectiveList
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public SolutionListOutput setObjectiveMinimizingObjectiveList(List<Boolean> isObjectiveToBeMinimized)
   :outertype: SolutionListOutput

setSeparator
^^^^^^^^^^^^

.. java:method:: public SolutionListOutput setSeparator(String separator)
   :outertype: SolutionListOutput

setVarFileOutputContext
^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public SolutionListOutput setVarFileOutputContext(FileOutputContext fileContext)
   :outertype: SolutionListOutput

