.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: org.uma.jmetal.util.fileoutput FileOutputContext

.. java:import:: java.io BufferedWriter

.. java:import:: java.io FileNotFoundException

.. java:import:: java.io FileOutputStream

.. java:import:: java.io OutputStreamWriter

DefaultFileOutputContext
========================

.. java:package:: org.uma.jmetal.util.fileoutput.impl
   :noindex:

.. java:type:: @SuppressWarnings public class DefaultFileOutputContext implements FileOutputContext

   Class using the default method for getting a buffered writer

   :author: Antonio J. Nebro

Fields
------
fileName
^^^^^^^^

.. java:field:: protected String fileName
   :outertype: DefaultFileOutputContext

separator
^^^^^^^^^

.. java:field:: protected String separator
   :outertype: DefaultFileOutputContext

Constructors
------------
DefaultFileOutputContext
^^^^^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public DefaultFileOutputContext(String fileName)
   :outertype: DefaultFileOutputContext

Methods
-------
getFileName
^^^^^^^^^^^

.. java:method:: @Override public String getFileName()
   :outertype: DefaultFileOutputContext

getFileWriter
^^^^^^^^^^^^^

.. java:method:: @Override public BufferedWriter getFileWriter()
   :outertype: DefaultFileOutputContext

getSeparator
^^^^^^^^^^^^

.. java:method:: @Override public String getSeparator()
   :outertype: DefaultFileOutputContext

setSeparator
^^^^^^^^^^^^

.. java:method:: @Override public void setSeparator(String separator)
   :outertype: DefaultFileOutputContext

