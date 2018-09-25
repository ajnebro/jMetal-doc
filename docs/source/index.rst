jMetal
==================

**jMetal** is an object-oriented Java-based framework for multi-objective optimization with metaheuristics
(http://jmetal.github.io/jMetal/).

This site contains documentation of the latest version of jMetal (version 5.6). The jMetal 5 project is hosted in GitHub: https://github.com/jMetal/jMetal

.. warning:: Documentation is WIP!! Some information may be missing.

.. toctree::
   :maxdepth: 1
   :caption: Contents:

   contributing
   documentation
   packages
   about


Introduction
------------------------

The jMetal project started in 2006 as the result of our need of having a easy to use, flexible, extensible and portable multi-objective optimization framework with metaheuristics. Since 2008 it has been hosted in http://jmetal.sourceforge.net. Since 2014 the current development is located in https://github.com/jMetal/jMetal.

After nine years since the first release of jMetal, we decided to make a deep redesign of the software in 2014. Some of the ideas taken into consideration were:

* Architecture redesign to provide a simpler design while keeping the same functionality.
* Maven is used as the tool for development, testing, packaging and deployment.
* Promote code reusing by providing algorithm templates
* Improve code quality:
  * Application of unit testing
  * Better use of Java features (e.g, generics)
  * Design patterns (singleton, builder, factory, observer)
  * Application of clean code guidelines - ''Clean code: A Handbook of Agile Software Craftsmanship'' (Robert C. Martin)
* Parallelism support
* Introducing measures to get information of the algorithms in runtime

The result was called jMetal 5, and a discussion about it can be found in the paper "Redesigning the jMetal Multi-Objective Optimization Framework. Antonio J. Nebro, Juan J. Durillo, Matthieu Vergne. GECCO (Companion) 2015". DOI: http://dx.doi.org/10.1145/2739482.2768462

Requirements
------------------------

jMetal is implemented in Java. Since version 5.2, we are using features of Java 8, so a Java 8 JDK or higher is required to compile the project.

As jMetal is a Maven project, this tool is also a requirement to compile, test and package the code.

Optionally, R and Latex are needed if you use the code to carry out experimental studies to run the R scripts and compile the Latex files that will be generated.

Compiling
------------------------

Once you have the source code of jMetal you can use it in to ways: from an IDE or from the command line of a terminal. The IDE alternative is the simplest one and, if you are used to the tool, compiling and running algorithms is easy.

Intellj Idea
~~~~~~~~~~~~~~~~~~~~~~

To build the project you have to select `Build` -> `Make Project`

![Building with IntelliJ Idea](https://github.com/jMetal/jMetalDocumentation/blob/master/figures/BuildIJICE14.png)


Eclipse
~~~~~~~~~~~~~~~~~~~~~~

If the `Project` -> `Build Automatically` is set, Eclipse will automatically build the project. Otherwise,  select  `Project` -> `Build Project`

![Building with Eclipse](https://github.com/jMetal/jMetalDocumentation/blob/master/figures/BuildEclipse.png)


Netbeans
~~~~~~~~~~~~~~~~~~~~~~

In Netbeans you have to select `Run` -> `Build Project`

![Building with Netbeans](https://github.com/jMetal/jMetalDocumentation/blob/master/figures/BuildNetbeans.png)

Building from the command line
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Once you have downloaded the source code you can use the command line to build the project by using Maven commands. If you open a terminal you will have something similar to this:

![jMetal in a terminal](https://github.com/jMetal/jMetalDocumentation/blob/master/figures/jMetalInTerminal.png)

Then you have Maven to your disposal to work with the project:
* `mvn clean`: cleaning the project
* `mvn compile`: compiling
* `mvn test`: testing
* `mvn package`: compiling, testing, generating documentation, and packaging in jar files
* `mvn site`: generates a site for the project
