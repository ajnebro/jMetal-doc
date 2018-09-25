<!--<div id='introduccion'/>-->

## Introduction 

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
