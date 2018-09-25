.. java:import:: org.uma.jmetal.operator.impl.crossover DifferentialEvolutionCrossover

.. java:import:: org.uma.jmetal.operator.impl.selection DifferentialEvolutionSelection

.. java:import:: org.uma.jmetal.problem DoubleProblem

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: org.uma.jmetal.util.evaluator SolutionListEvaluator

.. java:import:: org.uma.jmetal.util.evaluator.impl SequentialSolutionListEvaluator

DifferentialEvolutionBuilder
============================

.. java:package:: org.uma.jmetal.algorithm.singleobjective.differentialevolution
   :noindex:

.. java:type:: public class DifferentialEvolutionBuilder

   DifferentialEvolutionBuilder class

   :author: Antonio J. Nebro

Constructors
------------
DifferentialEvolutionBuilder
^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public DifferentialEvolutionBuilder(DoubleProblem problem)
   :outertype: DifferentialEvolutionBuilder

Methods
-------
build
^^^^^

.. java:method:: public DifferentialEvolution build()
   :outertype: DifferentialEvolutionBuilder

getCrossoverOperator
^^^^^^^^^^^^^^^^^^^^

.. java:method:: public DifferentialEvolutionCrossover getCrossoverOperator()
   :outertype: DifferentialEvolutionBuilder

getMaxEvaluations
^^^^^^^^^^^^^^^^^

.. java:method:: public int getMaxEvaluations()
   :outertype: DifferentialEvolutionBuilder

getPopulationSize
^^^^^^^^^^^^^^^^^

.. java:method:: public int getPopulationSize()
   :outertype: DifferentialEvolutionBuilder

getProblem
^^^^^^^^^^

.. java:method:: public DoubleProblem getProblem()
   :outertype: DifferentialEvolutionBuilder

getSelectionOperator
^^^^^^^^^^^^^^^^^^^^

.. java:method:: public DifferentialEvolutionSelection getSelectionOperator()
   :outertype: DifferentialEvolutionBuilder

getSolutionListEvaluator
^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public SolutionListEvaluator<DoubleSolution> getSolutionListEvaluator()
   :outertype: DifferentialEvolutionBuilder

setCrossover
^^^^^^^^^^^^

.. java:method:: public DifferentialEvolutionBuilder setCrossover(DifferentialEvolutionCrossover crossover)
   :outertype: DifferentialEvolutionBuilder

setMaxEvaluations
^^^^^^^^^^^^^^^^^

.. java:method:: public DifferentialEvolutionBuilder setMaxEvaluations(int maxEvaluations)
   :outertype: DifferentialEvolutionBuilder

setPopulationSize
^^^^^^^^^^^^^^^^^

.. java:method:: public DifferentialEvolutionBuilder setPopulationSize(int populationSize)
   :outertype: DifferentialEvolutionBuilder

setSelection
^^^^^^^^^^^^

.. java:method:: public DifferentialEvolutionBuilder setSelection(DifferentialEvolutionSelection selection)
   :outertype: DifferentialEvolutionBuilder

setSolutionListEvaluator
^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public DifferentialEvolutionBuilder setSolutionListEvaluator(SolutionListEvaluator<DoubleSolution> evaluator)
   :outertype: DifferentialEvolutionBuilder

