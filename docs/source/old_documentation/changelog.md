## Changelog 

### Version: jMetal 5.6

* Algorithms
  * Algorithm [SMPSO/RP](https://github.com/jMetal/jMetal/blob/master/jmetal-algorithm/src/main/java/org/uma/jmetal/algorithm/multiobjective/smpso/SMPSORP.java). 
  * Improvements in algorithms [WASF-GA](https://github.com/jMetal/jMetal/tree/master/jmetal-algorithm/src/main/java/org/uma/jmetal/algorithm/multiobjective/wasfga) and [GWASF-GA](https://github.com/jMetal/jMetal/tree/master/jmetal-algorithm/src/main/java/org/uma/jmetal/algorithm/multiobjective/gwasfga). Contribution of Rubén Saborido.
  * Algorithm MOEA/D and variants can now return a subset of evenly distributed solutions (see Miscelanea)
  * Algorithm [ESPEA](https://github.com/jMetal/jMetal/tree/master/jmetal-algorithm/src/main/java/org/uma/jmetal/algorithm/multiobjective/espea). Contribution of Marlon Braun.
  * Algorithm [CDG-MOEA](https://github.com/jMetal/jMetal/blob/master/jmetal-algorithm/src/main/java/org/uma/jmetal/algorithm/multiobjective/cdg/CDG.java). Contribution of Feng Zhang and Xinye Cai.

* Problems
  * Problems of the [CEC 2018 competition on many-objective optimization](https://github.com/jMetal/jMetal/tree/master/jmetal-problem/src/main/java/org/uma/jmetal/problem/multiobjective/maf). Contribution of Gian Mauricio Fritsche.

* Miscelanea
  * Added class [KNearestNeighborhood](https://github.com/jMetal/jMetal/blob/master/jmetal-core/src/main/java/org/uma/jmetal/util/neighborhood/impl/KNearestNeighborhood.java). 
  * Added new neighborhood classes: C25, C49, L13, L25 and L41 (https://github.com/jMetal/jMetal/tree/master/jmetal-core/src/main/java/org/uma/jmetal/util/neighborhood/impl).
  * Added method `getSubsetOfEvenlyDistributedSolutions()` to class [MOEADUtils](https://github.com/jMetal/jMetal/blob/master/jmetal-algorithm/src/main/java/org/uma/jmetal/algorithm/multiobjective/moead/util/MOEADUtils.java).

* Bugs
  * Fixed a bug in the component of the experiment package that executes the algorithms in parallel. All the experiment classes in package jmetal-exec have been updated.
  * Fixed a bug in the experiment framework which led to recompute quality indicators more times than needed.
  * Fixed a bug in class `AbstractGenericSolution` caused by solutions stored as attributes. This issue might lead to infinite recursive calls when two solutions are compared.


### Version: jMetal 5.4

* Algorithms
  * The algorithm R-NSGA-II (https://doi.org/10.1145/1143997.1144112) is available. Contribution of Cristóbal Barba (@cbarba).
  * Algorithm WASF-GA now can solve constrained problems (https://github.com/jMetal/jMetal/blob/master/jmetal-exec/src/main/java/org/uma/jmetal/runner/multiobjective/WASFGAConstraintRunner.java). Contribution of Cristóbal Barba (@cbarba).
  * Updated version of MOEA/DD and added a [runner class](https://github.com/jMetal/jMetal/blob/master/jmetal-exec/src/main/java/org/uma/jmetal/runner/multiobjective/MOEADDRunner.java) for it. Contribution of @fritsche.

* Operators
  * The `CrossoverOperator` interface contains a new method `numberOfGeneratedChildren()` and the former `getNumberOfParents()` has been renamed to `getNumberOfRequiredParents()`.

* Miscelanea
  * Added a [`WeightVectorNeighborhood`](https://github.com/jMetal/jMetal/blob/master/jmetal-core/src/main/java/org/uma/jmetal/util/neighborhood/impl/WeightVectorNeighborhood.java) class, which implements the [`Neighborhood`](https://github.com/jMetal/jMetal/blob/master/jmetal-core/src/main/java/org/uma/jmetal/util/neighborhood/Neighborhood.java) interface with the neighborhood scheme of MOEA/D.
  * Changed case of class names in CEC benchmark problems. Contribution of @leechristie

* Bugs
  * Algorithm WASF-GA now can solve problems with more than two objectives.

### Version: jMetal 5.3

* New algorithms
  * [MOEA/D-DD](http://ieeexplore.ieee.org/document/6964796/). Contribution of @vinixnan
  * Variants with measures of algorithms WASF-GA, DMOPSO, and SMPSO

* Quality indicators
  * The R2 indicator can be applied now to fronts with more than two objectives.

* Miscelanea
  * Class [ChartContainer](https://github.com/jMetal/jMetal/blob/master/jmetal-core/src/main/java/org/uma/jmetal/util/chartcontainer/ChartContainer.java), which is being developed by @georgero5. This class allows to display information of algorithms while they are running, such as the current Pareto front approximation or the evolution of indicators such as the Hypervolume. See classes [DMOPSOMeasuresRunner](https://github.com/jMetal/jMetal/blob/master/jmetal-exec/src/main/java/org/uma/jmetal/runner/multiobjective/DMOPSOMeasuresRunner.java) and [NSGAIIMeasuresWithChartsRunner](https://github.com/jMetal/jMetal/blob/master/jmetal-exec/src/main/java/org/uma/jmetal/runner/multiobjective/NSGAIIMeasuresWithChartsRunner.java) for examples using it.
  * Added getters and setters to all the parameters of the operators.
  * New interfaces for random generators based on functional interfaces.

* Bugs
  * Fixed a bug in algorithm MOEA/D


### Version: jMetal 5.2
From version 5.2, jmetal requires Java 8.

* New algorithms
 * [Coral Reef Optimization](https://github.com/jMetal/jMetal/tree/jmetal-5.2/jmetal-algorithm/src/main/java/org/uma/jmetal/algorithm/singleobjective/coralreefsoptimization)
 (S. Salcedo-Sanz, J. Del Ser, S. Gil-López, I. Landa-Torres and J. A. Portilla-Figueras, "The coral reefs optimization algorithm: an efficient meta-heuristic for solving hard optimization problems". 15th Applied Stochastic Models and Data Analysis International Conference, Mataró, Spain, June, 2013).
 Contribution of Inacio Medeiros

* New features
  * The classes related to experiments have been refactorized. 
  * Java 8 parallel streams are used to implement concurrency in the algorithms and in the experiments.

* Bugs fixed
  * Class [`Rosenbrock`](https://github.com/jMetal/jMetal/blob/master/jmetal-problem/src/main/java/org/uma/jmetal/problem/singleobjective/Rosenbrock.java) didn't set the lower and upper limits.
  * The default number of objectives in class [`UF9`](https://github.com/jMetal/jMetal/blob/master/jmetal-problem/src/main/java/org/uma/jmetal/problem/multiobjective/UF/UF9.java) was not correct.
  * A sentece was missing in class [`LZ09`](https://github.com/jMetal/jMetal/blob/master/jmetal-problem/src/main/java/org/uma/jmetal/problem/multiobjective/lz09/LZ09.java).
  * Fixed a bug in the `prune()` method of class `AdaptiveGridArchive` (thanks to SunnyWind).

### Version: jMetal 5.1
* New algorithms
 * [MOEADSTM](https://github.com/jMetal/jMetal/blob/master/jmetal-algorithm/src/main/java/org/uma/jmetal/algorithm/multiobjective/moead) 
 (K. Li, Q. Zhang, S. Kwong, M. Li and R. Wang, "Stable Matching-Based Selection in Evolutionary Multiobjective Optimization", IEEE Transactions on Evolutionary Computation, 18(6): 909-923, 2014. [10.1109/TEVC.2013.2293776](http://dx.doi.org/10.1109/TEVC.2013.2293776)).
Thanks to Ke Li for his contribution.
 * [MOCHC](https://github.com/jMetal/jMetal/tree/master/jmetal-algorithm/src/main/java/org/uma/jmetal/algorithm/multiobjective/mochc) 
 (Optimal antenna placement using a new multi-objective chc algorithm. A.J. Nebro, E. Alba, G. Molina, F. Chicano, F. Luna, J.J. Durillo. GECCO '07: Proceedings of the 9th annual conference on Genetic and evolutionary computation. London, England. July 2007. DOI: [10.1145/1276958.1277128](http://dx.doi.org/10.1145/1276958.1277128)) 
  * [MOMBI-II](https://github.com/jMetal/jMetal/tree/master/jmetal-algorithm/src/main/java/org/uma/jmetal/algorithm/multiobjective/mombi) (Improved Metaheuristic Based on the R2 Indicator for Many-Objective Optimization. R. Hernández Gómez, C.A. Coello Coello. Proceeding GECCO '15 Proceedings of the 2015 on Genetic and Evolutionary Computation Conference. Pages 679-686. DOI: [10.1145/2739480.2754776](http://dx.doi.org/10.1145/2739480.2754776)) 
  * [NSGA-III](https://github.com/jMetal/jMetal/tree/master/jmetal-algorithm/src/main/java/org/uma/jmetal/algorithm/multiobjective/nsgaiii) (Implementation based on the code of Tsung-Che Chiang: [http://web.ntnu.edu.tw/~tcchiang/publications/nsga3cpp/nsga3cpp.htm](http://web.ntnu.edu.tw/~tcchiang/publications/nsga3cpp/nsga3cpp.htm))
  * [WASF-GA](https://github.com/jMetal/jMetal/tree/master/jmetal-algorithm/src/main/java/org/uma/jmetal/algorithm/multiobjective/wasfga) (A Preference-based Evolutionary Algorithm for Multiobjective Optimization: The Weighting Achievement Scalarizing Function Genetic Algorithm. Journal of Global Optimization, May 2015, Volume 62, Issue 1, pp 101-129. DOI: [10.1007/s10898-014-0214-y](http://dx.doi.org/10.1007/s10898-014-0214-y)) 
  * [GWASF-GA](https://github.com/jMetal/jMetal/tree/master/jmetal-algorithm/src/main/java/org/uma/jmetal/algorithm/multiobjective/gwasfga) (Global WASF-GA: An Evolutionary Algorithm in Multiobjective Optimization to Approximate the whole Pareto Optimal Front. R. Saborido, A.B. Ruiz and M. Luque. Evolutionary Computation. Accepted for publication. 2015.) 
  * SMPSOhv: (Analysis of leader selection strategies in a multi-objective Particle Swarm Optimizer. A.J. Nebro, J.J. Durillo, C.A. Coello Coello. CEC 2013, June 2013, pp 3153-1360. DOI: [10.1109/CEC.2013.6557955](http://dx.doi.org/10.1109/CEC.2013.6557955)). Two variants can be configured depending on the [`HypervolumeArchive`](https://github.com/jMetal/jMetal/blob/master/jmetal-core/src/main/java/org/uma/jmetal/util/archive/impl/HypervolumeArchive.java), which can use a [`PISAHypervolume`](https://github.com/jMetal/jMetal/blob/master/jmetal-core/src/main/java/org/uma/jmetal/qualityindicator/impl/hypervolume/PISAHypervolume.java) or a [`WFGHypervolume`](https://github.com/jMetal/jMetal/blob/master/jmetal-core/src/main/java/org/uma/jmetal/qualityindicator/impl/hypervolume/WFGHypervolume.java) object.
  * [Standard PSO 2007](https://github.com/jMetal/jMetal/tree/master/jmetal-algorithm/src/main/java/org/uma/jmetal/algorithm/singleobjective/particleswarmoptimization) (single objective)
  * [Standard PSO 2011](https://github.com/jMetal/jMetal/tree/master/jmetal-algorithm/src/main/java/org/uma/jmetal/algorithm/singleobjective/particleswarmoptimization) (single objective)
  
* New benchmark problems
  * [GLT problems](https://github.com/jMetal/jMetal/tree/master/jmetal-problem/src/main/java/org/uma/jmetal/problem/multiobjective/glt). Defined in: F. Gu, H.-L. Liu, and K. C. Tan, “A multiobjective evolutionary algorithm using dynamic weight design method,” International Journal of Innovative Computing, Information and Control, vol. 8, no. 5B, pp. 3677–3688, 2012.
  * [MOP problems](https://github.com/jMetal/jMetal/tree/master/jmetal-problem/src/main/java/org/uma/jmetal/problem/multiobjective/mop). Defined in: H. L. Liu, F. Gu and Q. Zhang, "Decomposition of a Multiobjective Optimization Problem Into a Number of Simple Multiobjective Subproblems", in IEEE Transactions on Evolutionary Computation, vol. 18, no. 3, pp. 450-455, June 2014. Thanks to Mastermay for his contribution.

* New operators
  * [`BestSolutionSelection`](https://github.com/jMetal/jMetal/blob/master/jmetal-core/src/main/java/org/uma/jmetal/operator/impl/selection/BestSolutionSelection.java)

* New util classes
  * [`AdaptiveRandomNeighborhood`](https://github.com/jMetal/jMetal/blob/master/jmetal-core/src/main/java/org/uma/jmetal/util/neighborhood/impl/AdaptiveRandomNeighborhood.java)
  * [`HypervolumeArchive`](https://github.com/jMetal/jMetal/blob/master/jmetal-core/src/main/java/org/uma/jmetal/util/archive/impl/HypervolumeArchive.java)
 
* New features
  * Support for [experimental studies](https://github.com/jMetal/jMetal/tree/master/jmetal-exec/src/main/java/org/uma/jmetal/experiment)
    * Parallel algorithm execution.
    * Quality indicators computing.
    * Reference Pareto front approximations computing.
    * Generation of Latex tables:
      * Basic statistics (mean/median and standard deviation/IQR).
      * Wilcoxon rank sum test.
      * Friedman test ranking.
    * Generation of boxplots. 
  * Classes `PolynomialMutation` and `SBXCrossover` include setters to update their probability and distribution index values.
  * Two implementations of the [Hypervolume](https://github.com/jMetal/jMetal/blob/master/jmetal-core/src/main/java/org/uma/jmetal/qualityindicator/impl/Hypervolume.java) quality indicator are provided: [`PISAHypervolume`](https://github.com/jMetal/jMetal/blob/master/jmetal-core/src/main/java/org/uma/jmetal/qualityindicator/impl/hypervolume/PISAHypervolume.java) and [`WFGHypervolume`](https://github.com/jMetal/jMetal/blob/master/jmetal-core/src/main/java/org/uma/jmetal/qualityindicator/impl/hypervolume/WFGHypervolume.java)

* Bugs fixed
  * Fixed a bug in class [`DominanceComparator`](https://github.com/jMetal/jMetal/blob/master/jmetal-core/src/main/java/org/uma/jmetal/util/comparator/DominanceComparator.java)
