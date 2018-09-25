jMetal
======

jMetal stands for **Met**aheuristic **Al**gorithms in Java, and it is an object-oriented Java-based framework for multi-objective optimization with metaheuristics.

.. warning:: Documentation is WIP!! Some information may be missing.

.. toctree::
   :maxdepth: 1
   :caption: Contents:

   contributing
   installation
   documentation
   packages
   about

About jMetal 5
--------------

jMetal 5 is the first major revision of jMetal since its initial version. The architecture have been redesigned from scratch to provide a simpler design while keeping the same functionality. The current version is jMetal 5.6.

Now jMetal is a Maven project that is `hosted at GitHub <https://github.com/jMetal/jMetal>`_, where interested people can access to the current status of the project and are free to contribute.

The former jMetal versions are still `available at SourceForge <http://jmetal.sourceforge.net/>`_.

How to use it
-------------

You can find the last released versions of jMetal on the `Maven Central Repository <https://search.maven.org/search?q=g:org.uma.jmetal>`_.

To use jMetal in your project, you need at least the `jmetal-core` artifact.
It provides various components used to implement jMetal algorithms.
To implement your own, you only need this package.

jMetal comes with various algorithms already implemented, which you can obtain by adding the `jmetal-algorithm` artifact.
If you are more interested in experimenting with your own algorithms, you can instead add the `jmetal-problem` artifact to obtain various problems to solve.
You can of course add both of them to try combinations.
If you want to go further by running and evaluating different combinations, you can finally add the `jmetal-exec` artifact, which comes with various utilities.

Summary of features
-------------------

* Multi-objective algoritms: NSGA-II, SPEA2, PAES, PESA-II, OMOPSO, MOCell, AbYSS, MOEA/D, GDE3, IBEA, SMPSO, SMPSOhv, SMS-EMOA, MOEA/D-STM, MOEA/D-DE, MOCHC, MOMBI, MOMBI-II, NSGA-III, WASF-GA, GWASF-GA, R-NSGA-II, CDG-MOEA, ESPEA, SMSPO/RP
* Single-objective algoritms: genetic algorithm (variants: generational, steady-state), evolution strategy (variants: elitist or mu+lambda, non-elitist or mu, lambda), DE, CMA-ES, PSO (Stantard 2007, Standard 2011), Coral reef optimization.
* Algorithms that can be executed in parallel: NSGA-II, SMPSO, GDE3, SPEA2, PESA-II
* Included problems:
   * Problem families: ZDT, DTLZ, WFG, CEC2009, LZ09, GLT, MOP, CEC2018
   * Classical problems: Kursawe, Fonseca, Schaffer, Viennet2, Viennet3
   * Constrained problems: Srinivas, Tanaka, Osyczka2, Constr_Ex, Golinski, Water, Viennet4
   * Combinatorial problems: multi-objective TSP
   * Academic problems: OneMax, OneZeroMax
* Quality indicators: hypervolume, spread, generational distance, inverted generational distance, inverted generational distance plus, additive epsilon.
* Variable representations: binary, real, integer, permutation, mixed encoding (real+binary, int+real).