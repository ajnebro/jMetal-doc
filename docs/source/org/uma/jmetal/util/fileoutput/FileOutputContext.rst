.. java:import:: java.io BufferedWriter

.. java:import:: java.io Serializable

FileOutputContext
=================

.. java:package:: org.uma.jmetal.util.fileoutput
   :noindex:

.. java:type:: public interface FileOutputContext extends Serializable

   This interface represents output contexts, which are classes providing a mean for getting a buffer reader object.

   :author: Antonio J. Nebro

Methods
-------
getFileName
^^^^^^^^^^^

.. java:method:: public String getFileName()
   :outertype: FileOutputContext

getFileWriter
^^^^^^^^^^^^^

.. java:method:: public BufferedWriter getFileWriter()
   :outertype: FileOutputContext

getSeparator
^^^^^^^^^^^^

.. java:method:: public String getSeparator()
   :outertype: FileOutputContext

setSeparator
^^^^^^^^^^^^

.. java:method:: public void setSeparator(String separator)
   :outertype: FileOutputContext

