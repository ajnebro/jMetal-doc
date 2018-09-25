.. java:import:: org.uma.jmetal.measure PushMeasure

.. java:import:: org.uma.jmetal.measure.impl LastEvaluationMeasure.Evaluation

LastEvaluationMeasure
=====================

.. java:package:: org.uma.jmetal.measure.impl
   :noindex:

.. java:type:: @SuppressWarnings public class LastEvaluationMeasure<Solution, Value> extends SimplePushMeasure<Evaluation<Solution, Value>>

   \ :java:ref:`LastEvaluationMeasure`\  is a \ :java:ref:`PushMeasure`\  providing the last evaluation made in an algorithm. It extends \ :java:ref:`SimplePushMeasure`\  and add the method \ :java:ref:`push(Object,Object)`\  for simplicity.

   :author: Matthieu Vergne
   :param <Solution>: the solution evaluated
   :param <Value>: the type of value used to evaluate the solution (Double, BigDecimal, enum, ...)

Constructors
------------
LastEvaluationMeasure
^^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public LastEvaluationMeasure()
   :outertype: LastEvaluationMeasure

Methods
-------
push
^^^^

.. java:method:: public void push(Solution solution, Value value)
   :outertype: LastEvaluationMeasure

   This method is equivalent to \ :java:ref:`push(Object)`\  excepted that it automatically create the \ :java:ref:`Evaluation`\  instance.

   :param solution: the solution evaluated
   :param value: the value of this solution

