## Experimental studies

Since version 5.1, jMetal incorporates support for making experimental studies, i.e. configuring an experiment where a set of algorithms solve a number of problems and, as a result, a number of output files (latex tables, R scripts) are generated.

Some examples of experimental studies are included in jMetal 5.2:
* [NSGAIIStudy](https://github.com/jMetal/jMetal/blob/jmetal-5.2/jmetal-exec/src/main/java/org/uma/jmetal/experiment/NSGAIIStudy.java): four variants of NSGA-II (with different values of the polynomial mutation and SBX crossover distribution indexes) are tested to solve the five ZDT real-coded problems. The experiment carries out 25 inpendent runs per configuration and 8 cores are used.
* [NSGAIIStudy2](https://github.com/jMetal/jMetal/blob/jmetal-5.2/jmetal-exec/src/main/java/org/uma/jmetal/experiment/NSGAIIStudy2.java): the same as before but it is assumed that the reference Pareto fronts are not known, so they are obtained from all the fronts obtained by all the algorithms per problem; the contributio of each algorithm to the reference is also computed (only for continuous problems)
* [ZDTStudy](https://github.com/jMetal/jMetal/blob/jmetal-5.2/jmetal-exec/src/main/java/org/uma/jmetal/experiment/ZDTStudy.java): the same as `NSGAIIStudy` but three diffent algorithms are compared: NSGA-II, SPEA2 and SMPSO.
* [ZDTStudy2](https://github.com/jMetal/jMetal/blob/jmetal-5.2/jmetal-exec/src/main/java/org/uma/jmetal/experiment/ZDTStudy2.java): the same as before, but the reference Pareto fronts are computed as in `NSGAIIStudy`.
* [BinaryProblemsStudy](https://github.com/jMetal/jMetal/blob/jmetal-5.2/jmetal-exec/src/main/java/org/uma/jmetal/experiment/BinaryProblemsStudy.java): An example of experiment solving binary-coded problems.
* [ZDTScalabilityIStudy](https://github.com/jMetal/jMetal/blob/jmetal-5.2/jmetal-exec/src/main/java/org/uma/jmetal/experiment/ZDTScalabilityIStudy.java): This is an example of how using several variants of same problem in an experimental study. Concretely, this study is about solving five variants of the ZDT1 problem, each of them having a different number of decision variables. 
