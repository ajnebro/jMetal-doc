.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: org.uma.jmetal.util JMetalLogger

.. java:import:: java.io BufferedReader

.. java:import:: java.io FileInputStream

.. java:import:: java.io FileReader

.. java:import:: java.io InputStreamReader

.. java:import:: java.text DecimalFormat

.. java:import:: java.util Random

.. java:import:: java.util StringTokenizer

.. java:import:: java.util.logging Level

Benchmark
=========

.. java:package:: org.uma.jmetal.problem.singleobjective.cec2005competitioncode
   :noindex:

.. java:type:: public class Benchmark

Fields
------
CEC2005SUPPORTDATADIRECTORY
^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:field:: public static final String CEC2005SUPPORTDATADIRECTORY
   :outertype: Benchmark

DEFAULT_FILE_BIAS
^^^^^^^^^^^^^^^^^

.. java:field:: public static final String DEFAULT_FILE_BIAS
   :outertype: Benchmark

MAX_SUPPORT_DIM
^^^^^^^^^^^^^^^

.. java:field:: public static final int MAX_SUPPORT_DIM
   :outertype: Benchmark

NUM_TEST_FUNC
^^^^^^^^^^^^^

.. java:field:: public static final int NUM_TEST_FUNC
   :outertype: Benchmark

PIx2
^^^^

.. java:field:: public static final double PIx2
   :outertype: Benchmark

loader
^^^^^^

.. java:field:: public static final ClassLoader loader
   :outertype: Benchmark

numberFormatter
^^^^^^^^^^^^^^^

.. java:field:: public static final DecimalFormat numberFormatter
   :outertype: Benchmark

percentageFormatter
^^^^^^^^^^^^^^^^^^^

.. java:field:: public static final DecimalFormat percentageFormatter
   :outertype: Benchmark

random
^^^^^^

.. java:field:: public static final Random random
   :outertype: Benchmark

scientificFormatter
^^^^^^^^^^^^^^^^^^^

.. java:field:: public static final DecimalFormat scientificFormatter
   :outertype: Benchmark

test_func_arg_types
^^^^^^^^^^^^^^^^^^^

.. java:field:: static final Class<?>[] test_func_arg_types
   :outertype: Benchmark

test_func_class_names
^^^^^^^^^^^^^^^^^^^^^

.. java:field:: public static final String[] test_func_class_names
   :outertype: Benchmark

Constructors
------------
Benchmark
^^^^^^^^^

.. java:constructor:: public Benchmark() throws JMetalException
   :outertype: Benchmark

Benchmark
^^^^^^^^^

.. java:constructor:: public Benchmark(String file_bias) throws JMetalException
   :outertype: Benchmark

Methods
-------
Ax
^^

.. java:method:: public static void Ax(double[] result, double[][] A, double[] x)
   :outertype: Benchmark

EScafferF6
^^^^^^^^^^

.. java:method:: public static double EScafferF6(double[] x)
   :outertype: Benchmark

EScafferF6NonCont
^^^^^^^^^^^^^^^^^

.. java:method:: public static double EScafferF6NonCont(double[] x)
   :outertype: Benchmark

F2
^^

.. java:method:: public static double F2(double x, double y)
   :outertype: Benchmark

F8
^^

.. java:method:: public static double F8(double x)
   :outertype: Benchmark

F8F2
^^^^

.. java:method:: public static double F8F2(double[] x)
   :outertype: Benchmark

ScafferF6
^^^^^^^^^

.. java:method:: public static double ScafferF6(double x, double y)
   :outertype: Benchmark

ackley
^^^^^^

.. java:method:: public static double ackley(double[] x)
   :outertype: Benchmark

elliptic
^^^^^^^^

.. java:method:: public static double elliptic(double[] x)
   :outertype: Benchmark

griewank
^^^^^^^^

.. java:method:: public static double griewank(double[] x)
   :outertype: Benchmark

hybrid_composition
^^^^^^^^^^^^^^^^^^

.. java:method:: public static double hybrid_composition(double[] x, HCJob job) throws JMetalException
   :outertype: Benchmark

loadColumnVector
^^^^^^^^^^^^^^^^

.. java:method:: public static void loadColumnVector(BufferedReader brSrc, int rows, double[] column) throws Exception
   :outertype: Benchmark

loadColumnVectorFromFile
^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public static void loadColumnVectorFromFile(String file, int rows, double[] column) throws JMetalException
   :outertype: Benchmark

loadMatrix
^^^^^^^^^^

.. java:method:: public static void loadMatrix(BufferedReader brSrc, int rows, int columns, double[][] matrix) throws Exception
   :outertype: Benchmark

loadMatrixFromFile
^^^^^^^^^^^^^^^^^^

.. java:method:: public static void loadMatrixFromFile(String file, int rows, int columns, double[][] matrix) throws JMetalException
   :outertype: Benchmark

loadNMatrixFromFile
^^^^^^^^^^^^^^^^^^^

.. java:method:: public static void loadNMatrixFromFile(String file, int N, int rows, int columns, double[][][] matrix) throws JMetalException
   :outertype: Benchmark

loadRowVector
^^^^^^^^^^^^^

.. java:method:: public static void loadRowVector(BufferedReader brSrc, int columns, double[] row) throws Exception
   :outertype: Benchmark

loadRowVectorFromFile
^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public static void loadRowVectorFromFile(String file, int columns, double[] row) throws JMetalException
   :outertype: Benchmark

loadTestDataFromFile
^^^^^^^^^^^^^^^^^^^^

.. java:method:: public static void loadTestDataFromFile(String file, int num_test_points, int test_dimension, double[][] x, double[] f) throws JMetalException
   :outertype: Benchmark

main
^^^^

.. java:method:: public static void main(String[] args) throws JMetalException
   :outertype: Benchmark

myRound
^^^^^^^

.. java:method:: public static double myRound(double x)
   :outertype: Benchmark

myXRound
^^^^^^^^

.. java:method:: public static double myXRound(double x, double o)
   :outertype: Benchmark

myXRound
^^^^^^^^

.. java:method:: public static double myXRound(double x)
   :outertype: Benchmark

rastrigin
^^^^^^^^^

.. java:method:: public static double rastrigin(double[] x)
   :outertype: Benchmark

rastriginNonCont
^^^^^^^^^^^^^^^^

.. java:method:: public static double rastriginNonCont(double[] x)
   :outertype: Benchmark

rosenbrock
^^^^^^^^^^

.. java:method:: public static double rosenbrock(double[] x)
   :outertype: Benchmark

rotate
^^^^^^

.. java:method:: public static void rotate(double[] results, double[] x, double[][] matrix)
   :outertype: Benchmark

runTest
^^^^^^^

.. java:method:: public void runTest() throws JMetalException
   :outertype: Benchmark

runTest
^^^^^^^

.. java:method:: public void runTest(int func_num) throws JMetalException
   :outertype: Benchmark

schwefel_102
^^^^^^^^^^^^

.. java:method:: public static double schwefel_102(double[] x)
   :outertype: Benchmark

shift
^^^^^

.. java:method:: public static void shift(double[] results, double[] x, double[] o)
   :outertype: Benchmark

sphere
^^^^^^

.. java:method:: public static double sphere(double[] x)
   :outertype: Benchmark

sphere_noise
^^^^^^^^^^^^

.. java:method:: public static double sphere_noise(double[] x)
   :outertype: Benchmark

testFunctionFactory
^^^^^^^^^^^^^^^^^^^

.. java:method:: public TestFunc testFunctionFactory(int func_num, int dimension) throws JMetalException
   :outertype: Benchmark

weierstrass
^^^^^^^^^^^

.. java:method:: public static double weierstrass(double[] x)
   :outertype: Benchmark

weierstrass
^^^^^^^^^^^

.. java:method:: public static double weierstrass(double[] x, double a, double b, int Kmax)
   :outertype: Benchmark

xA
^^

.. java:method:: public static void xA(double[] result, double[] x, double[][] A)
   :outertype: Benchmark

xy
^^

.. java:method:: public static double xy(double[] x, double[] y)
   :outertype: Benchmark

