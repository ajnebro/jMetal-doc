.. java:import:: org.uma.jmetal.algorithm Algorithm

.. java:import:: java.util List

AbstractParticleSwarmOptimization
=================================

.. java:package:: org.uma.jmetal.algorithm.impl
   :noindex:

.. java:type:: @SuppressWarnings public abstract class AbstractParticleSwarmOptimization<S, Result> implements Algorithm<Result>

   Abstract class representing a PSO algorithm

   :author: Antonio J. Nebro

Methods
-------
createInitialSwarm
^^^^^^^^^^^^^^^^^^

.. java:method:: protected abstract List<S> createInitialSwarm()
   :outertype: AbstractParticleSwarmOptimization

evaluateSwarm
^^^^^^^^^^^^^

.. java:method:: protected abstract List<S> evaluateSwarm(List<S> swarm)
   :outertype: AbstractParticleSwarmOptimization

getResult
^^^^^^^^^

.. java:method:: @Override public abstract Result getResult()
   :outertype: AbstractParticleSwarmOptimization

getSwarm
^^^^^^^^

.. java:method:: public List<S> getSwarm()
   :outertype: AbstractParticleSwarmOptimization

initProgress
^^^^^^^^^^^^

.. java:method:: protected abstract void initProgress()
   :outertype: AbstractParticleSwarmOptimization

initializeLeader
^^^^^^^^^^^^^^^^

.. java:method:: protected abstract void initializeLeader(List<S> swarm)
   :outertype: AbstractParticleSwarmOptimization

initializeParticlesMemory
^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: protected abstract void initializeParticlesMemory(List<S> swarm)
   :outertype: AbstractParticleSwarmOptimization

initializeVelocity
^^^^^^^^^^^^^^^^^^

.. java:method:: protected abstract void initializeVelocity(List<S> swarm)
   :outertype: AbstractParticleSwarmOptimization

isStoppingConditionReached
^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: protected abstract boolean isStoppingConditionReached()
   :outertype: AbstractParticleSwarmOptimization

perturbation
^^^^^^^^^^^^

.. java:method:: protected abstract void perturbation(List<S> swarm)
   :outertype: AbstractParticleSwarmOptimization

run
^^^

.. java:method:: @Override public void run()
   :outertype: AbstractParticleSwarmOptimization

setSwarm
^^^^^^^^

.. java:method:: public void setSwarm(List<S> swarm)
   :outertype: AbstractParticleSwarmOptimization

updateLeaders
^^^^^^^^^^^^^

.. java:method:: protected abstract void updateLeaders(List<S> swarm)
   :outertype: AbstractParticleSwarmOptimization

updateParticlesMemory
^^^^^^^^^^^^^^^^^^^^^

.. java:method:: protected abstract void updateParticlesMemory(List<S> swarm)
   :outertype: AbstractParticleSwarmOptimization

updatePosition
^^^^^^^^^^^^^^

.. java:method:: protected abstract void updatePosition(List<S> swarm)
   :outertype: AbstractParticleSwarmOptimization

updateProgress
^^^^^^^^^^^^^^

.. java:method:: protected abstract void updateProgress()
   :outertype: AbstractParticleSwarmOptimization

updateVelocity
^^^^^^^^^^^^^^

.. java:method:: protected abstract void updateVelocity(List<S> swarm)
   :outertype: AbstractParticleSwarmOptimization

