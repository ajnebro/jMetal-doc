.. java:import:: org.knowm.xchart BitmapEncoder.BitmapFormat

.. java:import:: org.knowm.xchart XYSeries.XYSeriesRenderStyle

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.util.front.imp ArrayFront

.. java:import:: org.uma.jmetal.util.front.util FrontUtils

.. java:import:: java.io FileNotFoundException

.. java:import:: java.io IOException

.. java:import:: java.util List

.. java:import:: java.util.concurrent TimeUnit

ChartContainer
==============

.. java:package:: org.uma.jmetal.util.chartcontainer
   :noindex:

.. java:type:: public class ChartContainer

   Class for configuring and displaying a XChart.

   :author: Jorge Rodriguez Ordonez

Constructors
------------
ChartContainer
^^^^^^^^^^^^^^

.. java:constructor:: public ChartContainer(String name)
   :outertype: ChartContainer

ChartContainer
^^^^^^^^^^^^^^

.. java:constructor:: public ChartContainer(String name, int delay)
   :outertype: ChartContainer

Methods
-------
addIndicatorChart
^^^^^^^^^^^^^^^^^

.. java:method:: public void addIndicatorChart(String indicator)
   :outertype: ChartContainer

getChart
^^^^^^^^

.. java:method:: public XYChart getChart(String chartName)
   :outertype: ChartContainer

getDelay
^^^^^^^^

.. java:method:: public int getDelay()
   :outertype: ChartContainer

getFrontChart
^^^^^^^^^^^^^

.. java:method:: public XYChart getFrontChart()
   :outertype: ChartContainer

getName
^^^^^^^

.. java:method:: public String getName()
   :outertype: ChartContainer

getVarChart
^^^^^^^^^^^

.. java:method:: public XYChart getVarChart()
   :outertype: ChartContainer

initChart
^^^^^^^^^

.. java:method:: public void initChart()
   :outertype: ChartContainer

refreshCharts
^^^^^^^^^^^^^

.. java:method:: public void refreshCharts()
   :outertype: ChartContainer

refreshCharts
^^^^^^^^^^^^^

.. java:method:: public void refreshCharts(int delay)
   :outertype: ChartContainer

removeIndicator
^^^^^^^^^^^^^^^

.. java:method:: public void removeIndicator(String indicator)
   :outertype: ChartContainer

repaint
^^^^^^^

.. java:method:: public void repaint()
   :outertype: ChartContainer

saveChart
^^^^^^^^^

.. java:method:: public void saveChart(String fileName, BitmapFormat format) throws IOException
   :outertype: ChartContainer

setDelay
^^^^^^^^

.. java:method:: public ChartContainer setDelay(int delay)
   :outertype: ChartContainer

setFrontChart
^^^^^^^^^^^^^

.. java:method:: public void setFrontChart(int objective1, int objective2) throws FileNotFoundException
   :outertype: ChartContainer

setFrontChart
^^^^^^^^^^^^^

.. java:method:: public void setFrontChart(int objective1, int objective2, String referenceFrontFileName) throws FileNotFoundException
   :outertype: ChartContainer

setName
^^^^^^^

.. java:method:: public ChartContainer setName(String name)
   :outertype: ChartContainer

setReferencePoint
^^^^^^^^^^^^^^^^^

.. java:method:: public void setReferencePoint(List<Double> referencePoint)
   :outertype: ChartContainer

setVarChart
^^^^^^^^^^^

.. java:method:: public void setVarChart(int variable1, int variable2)
   :outertype: ChartContainer

updateFrontCharts
^^^^^^^^^^^^^^^^^

.. java:method:: public void updateFrontCharts(List<DoubleSolution> solutionList)
   :outertype: ChartContainer

updateIndicatorChart
^^^^^^^^^^^^^^^^^^^^

.. java:method:: public void updateIndicatorChart(String indicator, Double value)
   :outertype: ChartContainer

