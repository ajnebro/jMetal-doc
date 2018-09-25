.. java:import:: org.apache.commons.io FileUtils

.. java:import:: org.apache.commons.io IOUtils

.. java:import:: java.nio.charset Charset

.. java:import:: java.util.logging LogManager

.. java:import:: java.util.logging Logger

JMetalLogger
============

.. java:package:: org.uma.jmetal.util
   :noindex:

.. java:type:: @SuppressWarnings public class JMetalLogger implements Serializable

   This class provides some facilities to manage loggers. One might use the static logger of this class or use its own, custom logger. Also, we provide the static method \ :java:ref:`configureLoggers(File)`\  for configuring the loggers easily. This method is automatically called before any use of the static logger, but if you want it to apply on other loggers it is preferable to call it explicitly at the beginning of your main() method.

   :author: Antonio J. Nebro , Matthieu Vergne

Fields
------
logger
^^^^^^

.. java:field:: public static final Logger logger
   :outertype: JMetalLogger

Methods
-------
configureLoggers
^^^^^^^^^^^^^^^^

.. java:method:: public static void configureLoggers(File propertyFile) throws IOException
   :outertype: JMetalLogger

   This method provides a single-call method to configure the \ :java:ref:`Logger`\  instances. A default configuration is considered, enriched with a custom property file for more convenient logging. The custom file is considered after the default configuration, so it can override it if necessary. The custom file might be provided as an argument of this method, otherwise we look for a file named "jMetal.log.ini". If no custom file is provided, then only the default configuration is considered.

   :param propertyFile: the property file to use for custom configuration, \ ``null``\  to use only the default configuration
   :throws IOException:

