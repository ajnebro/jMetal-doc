.. java:import:: org.knowm.xchart BitmapEncoder.BitmapFormat

.. java:import:: org.knowm.xchart XYSeries.XYSeriesRenderStyle

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.util.front.imp ArrayFront

.. java:import:: org.uma.jmetal.util.front.util FrontUtils

.. java:import:: java.io FileNotFoundException

.. java:import:: java.io IOException

.. java:import:: java.util List

.. java:import:: java.util.concurrent TimeUnit

ChartContainerWithReferencePoints
=================================

.. java:package:: org.uma.jmetal.util.chartcontainer
   :noindex:

.. java:type:: public class ChartContainerWithReferencePoints

   Class for configuring and displaying a char with a number of subpopulations and reference points. Designed to be used with the SMPSORP.

   :author: Antonio J. Nebro

Constructors
------------
ChartContainerWithReferencePoints
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public ChartContainerWithReferencePoints(String name)
   :outertype: ChartContainerWithReferencePoints

ChartContainerWithReferencePoints
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:constructor:: public ChartContainerWithReferencePoints(String name, int delay)
   :outertype: ChartContainerWithReferencePoints

Methods
-------
getChart
^^^^^^^^

.. java:method:: public XYChart getChart(String chartName)
   :outertype: ChartContainerWithReferencePoints

getDelay
^^^^^^^^

.. java:method:: public int getDelay()
   :outertype: ChartContainerWithReferencePoints

getFrontChart
^^^^^^^^^^^^^

.. java:method:: public XYChart getFrontChart()
   :outertype: ChartContainerWithReferencePoints

getName
^^^^^^^

.. java:method:: public String getName()
   :outertype: ChartContainerWithReferencePoints

getVarChart
^^^^^^^^^^^

.. java:method:: public XYChart getVarChart()
   :outertype: ChartContainerWithReferencePoints

initChart
^^^^^^^^^

.. java:method:: public void initChart()
   :outertype: ChartContainerWithReferencePoints

refreshCharts
^^^^^^^^^^^^^

.. java:method:: public void refreshCharts()
   :outertype: ChartContainerWithReferencePoints

refreshCharts
^^^^^^^^^^^^^

.. java:method:: public void refreshCharts(int delay)
   :outertype: ChartContainerWithReferencePoints

repaint
^^^^^^^

.. java:method:: public void repaint()
   :outertype: ChartContainerWithReferencePoints

saveChart
^^^^^^^^^

.. java:method:: public void saveChart(String fileName, BitmapFormat format) throws IOException
   :outertype: ChartContainerWithReferencePoints

setDelay
^^^^^^^^

.. java:method:: public ChartContainerWithReferencePoints setDelay(int delay)
   :outertype: ChartContainerWithReferencePoints

setFrontChart
^^^^^^^^^^^^^

.. java:method:: public void setFrontChart(int objective1, int objective2) throws FileNotFoundException
   :outertype: ChartContainerWithReferencePoints

setFrontChart
^^^^^^^^^^^^^

.. java:method:: public void setFrontChart(int objective1, int objective2, String referenceFrontFileName) throws FileNotFoundException
   :outertype: ChartContainerWithReferencePoints

setName
^^^^^^^

.. java:method:: public ChartContainerWithReferencePoints setName(String name)
   :outertype: ChartContainerWithReferencePoints

setReferencePoint
^^^^^^^^^^^^^^^^^

.. java:method:: public synchronized void setReferencePoint(List<List<Double>> referencePoint)
   :outertype: ChartContainerWithReferencePoints

updateFrontCharts
^^^^^^^^^^^^^^^^^

.. java:method:: public void updateFrontCharts(List<DoubleSolution> solutionList)
   :outertype: ChartContainerWithReferencePoints

updateReferencePoint
^^^^^^^^^^^^^^^^^^^^

.. java:method:: public synchronized void updateReferencePoint(List<List<Double>> referencePoint)
   :outertype: ChartContainerWithReferencePoints

