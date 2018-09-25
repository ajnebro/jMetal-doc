.. java:import:: org.uma.jmetal.problem.impl AbstractDoubleProblem

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.solution.impl DefaultDoubleSolution

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: org.uma.jmetal.util.archive.impl NonDominatedSolutionListArchive

.. java:import:: org.uma.jmetal.util.fileoutput SolutionListOutput

.. java:import:: org.uma.jmetal.util.fileoutput.impl DefaultFileOutputContext

.. java:import:: java.io IOException

.. java:import:: java.nio.charset Charset

.. java:import:: java.nio.file Files

.. java:import:: java.nio.file Paths

.. java:import:: java.util ArrayList

.. java:import:: java.util List

.. java:import:: java.util.stream Stream

GenerateReferenceFrontFromFile
==============================

.. java:package:: org.uma.jmetal.utility
   :noindex:

.. java:type:: public class GenerateReferenceFrontFromFile

   This utility reads a file or the files in a directory and creates a reference front. The file(s) must contain only objective values. The program receives two parameters: 1. the name of the file or directory containing the data 2. the output file name which will contain the generated front

   :author: Antonio J. Nebro

Methods
-------
main
^^^^

.. java:method:: public static void main(String[] args) throws IOException
   :outertype: GenerateReferenceFrontFromFile

