.. java:import:: org.uma.jmetal.problem ConstrainedProblem

.. java:import:: org.uma.jmetal.problem.impl AbstractDoubleProblem

.. java:import:: org.uma.jmetal.solution DoubleSolution

.. java:import:: org.uma.jmetal.solution.impl DefaultDoubleSolution

.. java:import:: org.uma.jmetal.util JMetalException

.. java:import:: org.uma.jmetal.util.solutionattribute.impl OverallConstraintViolation

.. java:import:: java.util ArrayList

.. java:import:: java.util Arrays

.. java:import:: java.util Scanner

.. java:import:: java.util.logging Level

.. java:import:: java.util.logging Logger

Ebes
====

.. java:package:: org.uma.jmetal.problem.multiobjective.ebes
   :noindex:

.. java:type:: @SuppressWarnings public class Ebes extends AbstractDoubleProblem implements ConstrainedProblem<DoubleSolution>

   Class representing problem Ebes Spatial Bars Structure (Estructuras de Barras Espaciales)

Fields
------
AREA
^^^^

.. java:field::  int AREA
   :outertype: Ebes

ART_ART
^^^^^^^

.. java:field::  int ART_ART
   :outertype: Ebes

ART_RIG
^^^^^^^

.. java:field::  int ART_RIG
   :outertype: Ebes

AxialForcei_
^^^^^^^^^^^^

.. java:field:: protected double[] AxialForcei_
   :outertype: Ebes

   Stores the Axial force in node i

AxialForcej_
^^^^^^^^^^^^

.. java:field:: protected double[] AxialForcej_
   :outertype: Ebes

   Stores the Axial force in node j

Ay_
^^^

.. java:field::  int Ay_
   :outertype: Ebes

Az_
^^^

.. java:field::  int Az_
   :outertype: Ebes

BETA
^^^^

.. java:field::  int BETA
   :outertype: Ebes

BLijY_
^^^^^^

.. java:field::  int BLijY_
   :outertype: Ebes

BLijZ_
^^^^^^

.. java:field::  int BLijZ_
   :outertype: Ebes

CARGA_MOMENTO_DISTRIBUIDO
^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:field::  int CARGA_MOMENTO_DISTRIBUIDO
   :outertype: Ebes

CARGA_MOMENTO_PUNTUAL
^^^^^^^^^^^^^^^^^^^^^

.. java:field::  int CARGA_MOMENTO_PUNTUAL
   :outertype: Ebes

CARGA_PARABOLICA
^^^^^^^^^^^^^^^^

.. java:field::  int CARGA_PARABOLICA
   :outertype: Ebes

CARGA_PUNTUAL
^^^^^^^^^^^^^

.. java:field::  int CARGA_PUNTUAL
   :outertype: Ebes

CARGA_TEMPERATURA
^^^^^^^^^^^^^^^^^

.. java:field::  int CARGA_TEMPERATURA
   :outertype: Ebes

CARGA_TRIANGULAR_I
^^^^^^^^^^^^^^^^^^

.. java:field::  int CARGA_TRIANGULAR_I
   :outertype: Ebes

CARGA_UNIFORME_PARCIAL
^^^^^^^^^^^^^^^^^^^^^^

.. java:field::  int CARGA_UNIFORME_PARCIAL
   :outertype: Ebes

CARGA_UNIFORME_TOTAL
^^^^^^^^^^^^^^^^^^^^

.. java:field::  int CARGA_UNIFORME_TOTAL
   :outertype: Ebes

CARGA__TRIANGULAR_J
^^^^^^^^^^^^^^^^^^^

.. java:field::  int CARGA__TRIANGULAR_J
   :outertype: Ebes

CIRCLE
^^^^^^

.. java:field:: public static final int CIRCLE
   :outertype: Ebes

COMPRESSION
^^^^^^^^^^^

.. java:field::  int COMPRESSION
   :outertype: Ebes

CONSTRAINT
^^^^^^^^^^

.. java:field::  int CONSTRAINT
   :outertype: Ebes

DESCRIPTION
^^^^^^^^^^^

.. java:field::  int DESCRIPTION
   :outertype: Ebes

DisplacementNodes_
^^^^^^^^^^^^^^^^^^

.. java:field:: protected double[][] DisplacementNodes_
   :outertype: Ebes

   Stores the k displacement

ELONGATION_NEG
^^^^^^^^^^^^^^

.. java:field::  int ELONGATION_NEG
   :outertype: Ebes

ELONGATION_POS
^^^^^^^^^^^^^^

.. java:field::  int ELONGATION_POS
   :outertype: Ebes

E_
^^

.. java:field::  int E_
   :outertype: Ebes

Efforti_
^^^^^^^^

.. java:field:: protected double[][][] Efforti_
   :outertype: Ebes

   Stores the Effort in node i

Effortj_
^^^^^^^^

.. java:field:: protected double[][][] Effortj_
   :outertype: Ebes

   Stores the Effort in node j

Ei_
^^^

.. java:field::  int Ei_
   :outertype: Ebes

Ej_
^^^

.. java:field::  int Ej_
   :outertype: Ebes

Element_
^^^^^^^^

.. java:field:: protected double[][] Element_
   :outertype: Ebes

   Stores the Element

Fyz_
^^^^

.. java:field::  int Fyz_
   :outertype: Ebes

GROUP_
^^^^^^

.. java:field::  int GROUP_
   :outertype: Ebes

G_
^^

.. java:field::  int G_
   :outertype: Ebes

GravitationalAxis_
^^^^^^^^^^^^^^^^^^

.. java:field::  String GravitationalAxis_
   :outertype: Ebes

Groups_
^^^^^^^

.. java:field:: protected double[][] Groups_
   :outertype: Ebes

   Stores the Groups

HOLE_CIRCLE
^^^^^^^^^^^

.. java:field:: public static final int HOLE_CIRCLE
   :outertype: Ebes

HOLE_RECTANGLE
^^^^^^^^^^^^^^

.. java:field:: public static final int HOLE_RECTANGLE
   :outertype: Ebes

H_DOUBLE
^^^^^^^^

.. java:field:: public static final int H_DOUBLE
   :outertype: Ebes

H_SINGLE
^^^^^^^^

.. java:field:: public static final int H_SINGLE
   :outertype: Ebes

INDEX_
^^^^^^

.. java:field::  int INDEX_
   :outertype: Ebes

I_DOUBLE
^^^^^^^^

.. java:field:: public static final int I_DOUBLE
   :outertype: Ebes

I_SINGLE
^^^^^^^^

.. java:field:: public static final int I_SINGLE
   :outertype: Ebes

It_
^^^

.. java:field::  int It_
   :outertype: Ebes

Iw_
^^^

.. java:field::  int Iw_
   :outertype: Ebes

Iy_
^^^

.. java:field::  int Iy_
   :outertype: Ebes

Iz_
^^^

.. java:field::  int Iz_
   :outertype: Ebes

KGii
^^^^

.. java:field::  double[][] KGii
   :outertype: Ebes

KGij
^^^^

.. java:field::  double[][] KGij
   :outertype: Ebes

KGji
^^^^

.. java:field::  double[][] KGji
   :outertype: Ebes

KGjj
^^^^

.. java:field::  double[][] KGjj
   :outertype: Ebes

Kii
^^^

.. java:field::  double[][] Kii
   :outertype: Ebes

KiiSOG
^^^^^^

.. java:field::  double[][] KiiSOG
   :outertype: Ebes

Kij
^^^

.. java:field::  double[][] Kij
   :outertype: Ebes

KijSOG
^^^^^^

.. java:field::  double[][] KijSOG
   :outertype: Ebes

Kji
^^^

.. java:field::  double[][] Kji
   :outertype: Ebes

KjiSOG
^^^^^^

.. java:field::  double[][] KjiSOG
   :outertype: Ebes

Kjj
^^^

.. java:field::  double[][] Kjj
   :outertype: Ebes

KjjSOG
^^^^^^

.. java:field::  double[][] KjjSOG
   :outertype: Ebes

L_
^^

.. java:field::  int L_
   :outertype: Ebes

L_DOUBLE
^^^^^^^^

.. java:field:: public static final int L_DOUBLE
   :outertype: Ebes

L_SINGLE
^^^^^^^^

.. java:field:: public static final int L_SINGLE
   :outertype: Ebes

Li_
^^^

.. java:field::  int Li_
   :outertype: Ebes

Lj_
^^^

.. java:field::  int Lj_
   :outertype: Ebes

MAX_COLUMN
^^^^^^^^^^

.. java:field::  int MAX_COLUMN
   :outertype: Ebes

MatrixStiffness_
^^^^^^^^^^^^^^^^

.. java:field:: protected double[] MatrixStiffness_
   :outertype: Ebes

   Stores the k

MxyMax_
^^^^^^^

.. java:field:: protected double[][] MxyMax_
   :outertype: Ebes

   Stores the max Mxy for groups

MxyMin_
^^^^^^^

.. java:field:: protected double[][] MxyMin_
   :outertype: Ebes

   Stores the min Mxy for groups

MxzMax_
^^^^^^^

.. java:field:: protected double[][] MxzMax_
   :outertype: Ebes

   Stores the max Mxz for groups

MxzMin_
^^^^^^^

.. java:field:: protected double[][] MxzMin_
   :outertype: Ebes

   Stores the max Mxz for groups

NodeRestrict_
^^^^^^^^^^^^^

.. java:field:: protected double[][] NodeRestrict_
   :outertype: Ebes

   Stores the NodeRestrict

Node_
^^^^^

.. java:field:: protected double[][] Node_
   :outertype: Ebes

   Stores the Node

NxxMax_
^^^^^^^

.. java:field:: protected double[][] NxxMax_
   :outertype: Ebes

   Stores the max Nxx for groups

NxxMin_
^^^^^^^

.. java:field:: protected double[][] NxxMin_
   :outertype: Ebes

   Stores the min Nxx for groups

OF_
^^^

.. java:field::  String[] OF_
   :outertype: Ebes

OldStrainMax_
^^^^^^^^^^^^^

.. java:field:: protected double[][] OldStrainMax_
   :outertype: Ebes

   Stores the max Strain for elements

OldStrainMin_
^^^^^^^^^^^^^

.. java:field:: protected double[][] OldStrainMin_
   :outertype: Ebes

OverloadInElement_
^^^^^^^^^^^^^^^^^^

.. java:field:: protected double[][] OverloadInElement_
   :outertype: Ebes

   Stores the OverLoad on Elements

PQ
^^

.. java:field::  double[][] PQ
   :outertype: Ebes

QAx_
^^^^

.. java:field::  int QAx_
   :outertype: Ebes

QAy_
^^^^

.. java:field::  int QAy_
   :outertype: Ebes

QAz_
^^^^

.. java:field::  int QAz_
   :outertype: Ebes

QE_
^^^

.. java:field::  int QE_
   :outertype: Ebes

QH_
^^^

.. java:field::  int QH_
   :outertype: Ebes

QT_
^^^

.. java:field::  int QT_
   :outertype: Ebes

Qa_
^^^

.. java:field::  int Qa_
   :outertype: Ebes

Qb_
^^^

.. java:field::  int Qb_
   :outertype: Ebes

Qi
^^

.. java:field::  double[] Qi
   :outertype: Ebes

Qj
^^

.. java:field::  double[] Qj
   :outertype: Ebes

RATIO_YZ
^^^^^^^^

.. java:field::  int RATIO_YZ
   :outertype: Ebes

RECTANGLE
^^^^^^^^^

.. java:field:: public static final int RECTANGLE
   :outertype: Ebes

RIG_ART
^^^^^^^

.. java:field::  int RIG_ART
   :outertype: Ebes

RIG_RIG
^^^^^^^

.. java:field::  int RIG_RIG
   :outertype: Ebes

RTij
^^^^

.. java:field::  double[][] RTij
   :outertype: Ebes

RTji
^^^^

.. java:field::  double[][] RTji
   :outertype: Ebes

Reaction_
^^^^^^^^^

.. java:field::  double Reaction_
   :outertype: Ebes

Rij
^^^

.. java:field::  double[][] Rij
   :outertype: Ebes

Rji
^^^

.. java:field::  double[][] Rji
   :outertype: Ebes

RpTij
^^^^^

.. java:field::  double[][] RpTij
   :outertype: Ebes

RpTji
^^^^^

.. java:field::  double[][] RpTji
   :outertype: Ebes

Rpij
^^^^

.. java:field::  double[][] Rpij
   :outertype: Ebes

Rpji
^^^^

.. java:field::  double[][] Rpji
   :outertype: Ebes

SHAPE
^^^^^

.. java:field::  int SHAPE
   :outertype: Ebes

SPECIFIC_WEIGHT
^^^^^^^^^^^^^^^

.. java:field::  int SPECIFIC_WEIGHT
   :outertype: Ebes

STRAIN_COMPRESS
^^^^^^^^^^^^^^^

.. java:field::  int STRAIN_COMPRESS
   :outertype: Ebes

STRAIN_CUT
^^^^^^^^^^

.. java:field::  int STRAIN_CUT
   :outertype: Ebes

STRAIN_TRACTION
^^^^^^^^^^^^^^^

.. java:field::  int STRAIN_TRACTION
   :outertype: Ebes

STRESS
^^^^^^

.. java:field::  int STRESS
   :outertype: Ebes

STRESS_CUT
^^^^^^^^^^

.. java:field::  int STRESS_CUT
   :outertype: Ebes

StrainCutMax_
^^^^^^^^^^^^^

.. java:field:: protected double[][] StrainCutMax_
   :outertype: Ebes

   Stores the max Strain for elements

StrainMax_
^^^^^^^^^^

.. java:field:: protected double[][] StrainMax_
   :outertype: Ebes

   Stores the max Strain for elements

StrainMin_
^^^^^^^^^^

.. java:field:: protected double[][] StrainMin_
   :outertype: Ebes

StrainMxyMax_
^^^^^^^^^^^^^

.. java:field:: protected double[][] StrainMxyMax_
   :outertype: Ebes

   Stores the max Mxz Strain for groups

StrainMxyMin_
^^^^^^^^^^^^^

.. java:field:: protected double[][] StrainMxyMin_
   :outertype: Ebes

   Stores the max Mxz Strain for groups

StrainMxzMax_
^^^^^^^^^^^^^

.. java:field:: protected double[][] StrainMxzMax_
   :outertype: Ebes

   Stores the max Mxz Strain for groups

StrainMxzMin_
^^^^^^^^^^^^^

.. java:field:: protected double[][] StrainMxzMin_
   :outertype: Ebes

   Stores the max Mxz Strain for groups

StrainNxxMax_
^^^^^^^^^^^^^

.. java:field:: protected double[][] StrainNxxMax_
   :outertype: Ebes

   Stores the max Nxx Strain for groups

StrainNxxMin_
^^^^^^^^^^^^^

.. java:field:: protected double[][] StrainNxxMin_
   :outertype: Ebes

StrainResidualCut_
^^^^^^^^^^^^^^^^^^

.. java:field:: protected double[] StrainResidualCut_
   :outertype: Ebes

   Stores the Cut Strain Residual for elements

StrainResidualMax_
^^^^^^^^^^^^^^^^^^

.. java:field:: protected double[] StrainResidualMax_
   :outertype: Ebes

   Stores the max Strain for elements

StrainResidualMin_
^^^^^^^^^^^^^^^^^^

.. java:field:: protected double[] StrainResidualMin_
   :outertype: Ebes

   Stores the min Strain for elements

Straini_
^^^^^^^^

.. java:field:: protected double[][][] Straini_
   :outertype: Ebes

   Stores the Strain in node i

Strainj_
^^^^^^^^

.. java:field:: protected double[][][] Strainj_
   :outertype: Ebes

   Stores the Strain in node j

T_DOUBLE
^^^^^^^^

.. java:field:: public static final int T_DOUBLE
   :outertype: Ebes

T_SINGLE
^^^^^^^^

.. java:field:: public static final int T_SINGLE
   :outertype: Ebes

TypeMaterial_
^^^^^^^^^^^^^

.. java:field::  int TypeMaterial_
   :outertype: Ebes

VARIABLES
^^^^^^^^^

.. java:field::  int VARIABLES
   :outertype: Ebes

VAR_POSITION
^^^^^^^^^^^^

.. java:field::  int VAR_POSITION
   :outertype: Ebes

VAR_Y_LOWER_LIMIT
^^^^^^^^^^^^^^^^^

.. java:field::  int VAR_Y_LOWER_LIMIT
   :outertype: Ebes

VAR_Y_UPPER_LIMIT
^^^^^^^^^^^^^^^^^

.. java:field::  int VAR_Y_UPPER_LIMIT
   :outertype: Ebes

VAR_Z_LOWER_LIMIT
^^^^^^^^^^^^^^^^^

.. java:field::  int VAR_Z_LOWER_LIMIT
   :outertype: Ebes

VAR_Z_UPPER_LIMIT
^^^^^^^^^^^^^^^^^

.. java:field::  int VAR_Z_UPPER_LIMIT
   :outertype: Ebes

VAR_eY_LOWER_LIMIT
^^^^^^^^^^^^^^^^^^

.. java:field::  int VAR_eY_LOWER_LIMIT
   :outertype: Ebes

VAR_eY_UPPER_LIMIT
^^^^^^^^^^^^^^^^^^

.. java:field::  int VAR_eY_UPPER_LIMIT
   :outertype: Ebes

VAR_eZ_LOWER_LIMIT
^^^^^^^^^^^^^^^^^^

.. java:field::  int VAR_eZ_LOWER_LIMIT
   :outertype: Ebes

VAR_eZ_UPPER_LIMIT
^^^^^^^^^^^^^^^^^^

.. java:field::  int VAR_eZ_UPPER_LIMIT
   :outertype: Ebes

Vij_
^^^^

.. java:field::  int Vij_
   :outertype: Ebes

WeightElement_
^^^^^^^^^^^^^^

.. java:field:: protected double[][] WeightElement_
   :outertype: Ebes

   Stores the Load on Elements Itself

WeightNode_
^^^^^^^^^^^

.. java:field:: protected double[][] WeightNode_
   :outertype: Ebes

   Stores the Load on Nodes

Y_
^^

.. java:field::  int Y_
   :outertype: Ebes

Z_
^^

.. java:field::  int Z_
   :outertype: Ebes

aX_
^^^

.. java:field::  int aX_
   :outertype: Ebes

aY_
^^^

.. java:field::  int aY_
   :outertype: Ebes

aZ_
^^^

.. java:field::  int aZ_
   :outertype: Ebes

cbi
^^^

.. java:field::  double[][][] cbi
   :outertype: Ebes

cbj
^^^

.. java:field::  double[][][] cbj
   :outertype: Ebes

dY_
^^^

.. java:field::  int dY_
   :outertype: Ebes

eY_
^^^

.. java:field::  int eY_
   :outertype: Ebes

eZ_
^^^

.. java:field::  int eZ_
   :outertype: Ebes

elementsBetweenDiffGreat_
^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:field:: protected int elementsBetweenDiffGreat_
   :outertype: Ebes

   Stores the Elements Between Difference Greatest

gX_
^^^

.. java:field::  int gX_
   :outertype: Ebes

gY_
^^^

.. java:field::  int gY_
   :outertype: Ebes

gZ_
^^^

.. java:field::  int gZ_
   :outertype: Ebes

g_
^^

.. java:field::  double g_
   :outertype: Ebes

geometryCheck_
^^^^^^^^^^^^^^

.. java:field:: protected int[][] geometryCheck_
   :outertype: Ebes

i_
^^

.. java:field::  int i_
   :outertype: Ebes

j_
^^

.. java:field::  int j_
   :outertype: Ebes

lBuckling
^^^^^^^^^

.. java:field:: public boolean lBuckling
   :outertype: Ebes

lLoadsOwnWeight
^^^^^^^^^^^^^^^

.. java:field:: public boolean lLoadsOwnWeight
   :outertype: Ebes

lSecondOrderGeometric
^^^^^^^^^^^^^^^^^^^^^

.. java:field:: public boolean lSecondOrderGeometric
   :outertype: Ebes

lZ_
^^^

.. java:field::  int lZ_
   :outertype: Ebes

matrixWidthBand_
^^^^^^^^^^^^^^^^

.. java:field:: protected int matrixWidthBand_
   :outertype: Ebes

   Stores the number a wide the diagonal matrix

nodeCheck_
^^^^^^^^^^

.. java:field:: protected double[][] nodeCheck_
   :outertype: Ebes

   Stores the number of Nodes of the problem

numberOfConstraintsGeometric_
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:field:: public int numberOfConstraintsGeometric_
   :outertype: Ebes

numberOfConstraintsNodes_
^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:field:: protected int numberOfConstraintsNodes_
   :outertype: Ebes

numberOfElements_
^^^^^^^^^^^^^^^^^

.. java:field:: protected int numberOfElements_
   :outertype: Ebes

   Stores the number of Bar of the problem

numberOfEval_
^^^^^^^^^^^^^

.. java:field:: protected int numberOfEval_
   :outertype: Ebes

   Stores the number of Bar Groups

numberOfGroupElements_
^^^^^^^^^^^^^^^^^^^^^^

.. java:field:: protected int numberOfGroupElements_
   :outertype: Ebes

   Stores the number of Bar Groups

numberOfGroupsToCheckGeometry_
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:field:: protected int numberOfGroupsToCheckGeometry_
   :outertype: Ebes

numberOfLibertyDegree_
^^^^^^^^^^^^^^^^^^^^^^

.. java:field:: protected int numberOfLibertyDegree_
   :outertype: Ebes

   Stores the number of Nodes of the problem

numberOfNodes
^^^^^^^^^^^^^

.. java:field:: protected int numberOfNodes
   :outertype: Ebes

numberOfNodesRestricts_
^^^^^^^^^^^^^^^^^^^^^^^

.. java:field:: protected int numberOfNodesRestricts_
   :outertype: Ebes

numberOfWeigthHypothesis_
^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:field:: protected int numberOfWeigthHypothesis_
   :outertype: Ebes

numberOfWeigthsElements_
^^^^^^^^^^^^^^^^^^^^^^^^

.. java:field:: protected int numberOfWeigthsElements_
   :outertype: Ebes

   Stores the number of Load in ElementsNodes of the problem

numberOfWeigthsNodes_
^^^^^^^^^^^^^^^^^^^^^

.. java:field:: protected int numberOfWeigthsNodes_
   :outertype: Ebes

   Stores the number of Load in Nodes of the problem

omegaMax_
^^^^^^^^^

.. java:field:: protected double[][] omegaMax_
   :outertype: Ebes

   Stores the max omega for groups

overallConstraintViolationDegree
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:field:: public OverallConstraintViolation<DoubleSolution> overallConstraintViolationDegree
   :outertype: Ebes

pi
^^

.. java:field::  double[] pi
   :outertype: Ebes

pj
^^

.. java:field::  double[] pj
   :outertype: Ebes

rZ_
^^^

.. java:field::  int rZ_
   :outertype: Ebes

selectedOF
^^^^^^^^^^

.. java:field::  int selectedOF
   :outertype: Ebes

strainAdmissibleCut_
^^^^^^^^^^^^^^^^^^^^

.. java:field:: protected int strainAdmissibleCut_
   :outertype: Ebes

uY_
^^^

.. java:field::  int uY_
   :outertype: Ebes

Constructors
------------
Ebes
^^^^

.. java:constructor:: public Ebes() throws FileNotFoundException
   :outertype: Ebes

Ebes
^^^^

.. java:constructor:: public Ebes(String ebesFileName, String[] objectiveList) throws FileNotFoundException
   :outertype: Ebes

   Constructor

   :throws FileNotFoundException:

Methods
-------
AxialForcei_
^^^^^^^^^^^^

.. java:method:: public double AxialForcei_(int element)
   :outertype: Ebes

AxialForcej_
^^^^^^^^^^^^

.. java:method:: public double AxialForcej_(int element)
   :outertype: Ebes

BucklingOmega
^^^^^^^^^^^^^

.. java:method:: public double BucklingOmega(double Nxx, double[] G, double[] B) throws JMetalException
   :outertype: Ebes

DisplacementNodes
^^^^^^^^^^^^^^^^^

.. java:method:: public double DisplacementNodes(int node, int hi)
   :outertype: Ebes

EBEsAssignAxialForces
^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public void EBEsAssignAxialForces(int hi)
   :outertype: Ebes

EBEsCalculus
^^^^^^^^^^^^

.. java:method:: public void EBEsCalculus() throws JMetalException
   :outertype: Ebes

EBEsEcuationSolution
^^^^^^^^^^^^^^^^^^^^

.. java:method:: public void EBEsEcuationSolution(int hi) throws JMetalException
   :outertype: Ebes

EBEsEffortsElements3D
^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public void EBEsEffortsElements3D(int hi, int countIter, double[][] Slip) throws JMetalException
   :outertype: Ebes

EBEsEffortsTotal3D
^^^^^^^^^^^^^^^^^^

.. java:method:: public void EBEsEffortsTotal3D(int hi)
   :outertype: Ebes

EBEsElementsTopology
^^^^^^^^^^^^^^^^^^^^

.. java:method:: public void EBEsElementsTopology(DoubleSolution solution) throws JMetalException
   :outertype: Ebes

EBEsInitialize
^^^^^^^^^^^^^^

.. java:method:: public void EBEsInitialize(String file) throws FileNotFoundException
   :outertype: Ebes

EBEsMat3DG
^^^^^^^^^^

.. java:method:: public void EBEsMat3DG(int e) throws JMetalException
   :outertype: Ebes

EBEsMat3DGij
^^^^^^^^^^^^

.. java:method:: public void EBEsMat3DGij() throws JMetalException
   :outertype: Ebes

EBEsMat3DL_SOG
^^^^^^^^^^^^^^

.. java:method:: public void EBEsMat3DL_SOG(int e) throws JMetalException
   :outertype: Ebes

EBEsMat3DL_iArt_jArt
^^^^^^^^^^^^^^^^^^^^

.. java:method:: public void EBEsMat3DL_iArt_jArt(int e) throws JMetalException
   :outertype: Ebes

EBEsMat3DL_iArt_jRig
^^^^^^^^^^^^^^^^^^^^

.. java:method:: public void EBEsMat3DL_iArt_jRig(int e) throws JMetalException
   :outertype: Ebes

EBEsMat3DL_iRig_jArt
^^^^^^^^^^^^^^^^^^^^

.. java:method:: public void EBEsMat3DL_iRig_jArt(int e) throws JMetalException
   :outertype: Ebes

EBEsMat3DL_iRig_jRig
^^^^^^^^^^^^^^^^^^^^

.. java:method:: public void EBEsMat3DL_iRig_jRig(int e) throws JMetalException
   :outertype: Ebes

EBEsMatRot3DLaG
^^^^^^^^^^^^^^^

.. java:method:: public void EBEsMatRot3DLaG(int e) throws JMetalException
   :outertype: Ebes

EBEsMatRot3DLpSaL
^^^^^^^^^^^^^^^^^

.. java:method:: public void EBEsMatRot3DLpSaL(int e)
   :outertype: Ebes

EBEsMatrixAdd
^^^^^^^^^^^^^

.. java:method:: public double[][] EBEsMatrixAdd(double[][] s, double[][] t) throws JMetalException
   :outertype: Ebes

EBEsMatrixGlobalFactory
^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public void EBEsMatrixGlobalFactory(int countIter) throws JMetalException
   :outertype: Ebes

EBEsMatrixGlobalPenalization
^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public void EBEsMatrixGlobalPenalization()
   :outertype: Ebes

EBEsMatrixSubtractions
^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public double[][] EBEsMatrixSubtractions(double[][] s, double[][] t) throws JMetalException
   :outertype: Ebes

EBEsMatrixWeight
^^^^^^^^^^^^^^^^

.. java:method:: public void EBEsMatrixWeight(int hi)
   :outertype: Ebes

EBEsMatrizMultiplicar
^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public double[][] EBEsMatrizMultiplicar(double[][] s, double[][] t) throws JMetalException
   :outertype: Ebes

EBEsMatrizTraspuesta
^^^^^^^^^^^^^^^^^^^^

.. java:method:: public double[][] EBEsMatrizTraspuesta(double[][] m)
   :outertype: Ebes

EBEsMatrizVectorMultiplicar
^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public double[] EBEsMatrizVectorMultiplicar(double[][] s, double[] t) throws JMetalException
   :outertype: Ebes

EBEsNodesEquilibrium3D
^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public void EBEsNodesEquilibrium3D(int hi) throws JMetalException
   :outertype: Ebes

EBEsOverloadWeightElement
^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public void EBEsOverloadWeightElement() throws JMetalException
   :outertype: Ebes

EBEsPrintArchTxtDesp
^^^^^^^^^^^^^^^^^^^^

.. java:method:: public void EBEsPrintArchTxtDesp(int hi) throws JMetalException
   :outertype: Ebes

EBEsPrintArchTxtEfforts
^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public void EBEsPrintArchTxtEfforts(int hi) throws JMetalException
   :outertype: Ebes

EBEsPrintArchTxtElements
^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public void EBEsPrintArchTxtElements() throws JMetalException
   :outertype: Ebes

EBEsPrintArchTxtMKG
^^^^^^^^^^^^^^^^^^^

.. java:method:: public void EBEsPrintArchTxtMKG(String s, int hi) throws JMetalException
   :outertype: Ebes

EBEsPrintArchTxtMKLB
^^^^^^^^^^^^^^^^^^^^

.. java:method:: public void EBEsPrintArchTxtMKLB(int e) throws JMetalException
   :outertype: Ebes

EBEsPrintArchTxtReaction
^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public void EBEsPrintArchTxtReaction(int hi) throws JMetalException
   :outertype: Ebes

EBEsPrintArchTxtStrain
^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public void EBEsPrintArchTxtStrain() throws JMetalException
   :outertype: Ebes

EBEsReactions3D
^^^^^^^^^^^^^^^

.. java:method:: public void EBEsReactions3D(int hi)
   :outertype: Ebes

EBEsReadDataFile
^^^^^^^^^^^^^^^^

.. java:method:: public final void EBEsReadDataFile(String fileName) throws JMetalException
   :outertype: Ebes

EBEsReadProblems
^^^^^^^^^^^^^^^^

.. java:method:: public String EBEsReadProblems() throws FileNotFoundException
   :outertype: Ebes

EBEsSteelingResults
^^^^^^^^^^^^^^^^^^^

.. java:method:: public void EBEsSteelingResults(int hi)
   :outertype: Ebes

EBEsStrainMaxWhitElement
^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public void EBEsStrainMaxWhitElement() throws JMetalException
   :outertype: Ebes

EBEsStrainMaxWhitGroup
^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public void EBEsStrainMaxWhitGroup() throws JMetalException
   :outertype: Ebes

EBEsStrainMinWhitElement
^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public void EBEsStrainMinWhitElement() throws JMetalException
   :outertype: Ebes

EBEsStrainMinWhitGroup
^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public void EBEsStrainMinWhitGroup() throws JMetalException
   :outertype: Ebes

EBEsStrainNode
^^^^^^^^^^^^^^

.. java:method:: public double[][][] EBEsStrainNode(double[][][] E) throws JMetalException
   :outertype: Ebes

EBEsStrainResidualVerication
^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public void EBEsStrainResidualVerication() throws JMetalException
   :outertype: Ebes

EBEsTransversalSectionCircular
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public void EBEsTransversalSectionCircular(int gr, double d) throws JMetalException
   :outertype: Ebes

EBEsTransversalSectionHoleCircular
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public void EBEsTransversalSectionHoleCircular(int gr, double D, double e) throws JMetalException
   :outertype: Ebes

EBEsTransversalSectionHoleRectangle
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public void EBEsTransversalSectionHoleRectangle(int gr, double y, double z, double ey, double ez) throws JMetalException
   :outertype: Ebes

EBEsTransversalSectionRectangle
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public void EBEsTransversalSectionRectangle(int gr, double y, double z) throws JMetalException
   :outertype: Ebes

EBEsTransversalSection_H_Double
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public void EBEsTransversalSection_H_Double(int gr, double y, double z, double ey, double ez) throws JMetalException
   :outertype: Ebes

EBEsTransversalSection_H_Single
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public void EBEsTransversalSection_H_Single(int gr, double y, double z, double ey, double ez) throws JMetalException
   :outertype: Ebes

EBEsTransversalSection_I_Double
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public void EBEsTransversalSection_I_Double(int gr, double y, double z, double ey, double ez) throws JMetalException
   :outertype: Ebes

EBEsTransversalSection_I_Single
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public void EBEsTransversalSection_I_Single(int gr, double y, double z, double ey, double ez) throws JMetalException
   :outertype: Ebes

EBEsTransversalSection_L_Double
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public void EBEsTransversalSection_L_Double(int gr, double y, double z, double ey, double ez) throws JMetalException
   :outertype: Ebes

EBEsTransversalSection_L_Single
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public void EBEsTransversalSection_L_Single(int gr, double y, double z, double ey, double ez) throws JMetalException
   :outertype: Ebes

EBEsTransversalSection_T_Double
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public void EBEsTransversalSection_T_Double(int ba, double y, double z, double ey, double ez) throws JMetalException
   :outertype: Ebes

EBEsTransversalSection_T_Single
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public void EBEsTransversalSection_T_Single(int ba, double y, double z, double ey, double ez) throws JMetalException
   :outertype: Ebes

EBEsWeightDistributedUniformly
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public void EBEsWeightDistributedUniformly(int el, double[] LoadInElement_) throws JMetalException
   :outertype: Ebes

EBEsWeightNodes
^^^^^^^^^^^^^^^

.. java:method:: public void EBEsWeightNodes()
   :outertype: Ebes

EBEsWeigthElement
^^^^^^^^^^^^^^^^^

.. java:method:: public void EBEsWeigthElement() throws JMetalException
   :outertype: Ebes

Efforti
^^^^^^^

.. java:method:: public double Efforti(int i, int element, int hypothesis)
   :outertype: Ebes

Effortj
^^^^^^^

.. java:method:: public double Effortj(int i, int element, int hypothesis)
   :outertype: Ebes

FunctionENS
^^^^^^^^^^^

.. java:method:: public double FunctionENS(int hi)
   :outertype: Ebes

FunctionsMahalanobis_Distance_With_Variance
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public double FunctionsMahalanobis_Distance_With_Variance(int hi)
   :outertype: Ebes

Interpolation_I_Single_Y_func_Area_
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public double Interpolation_I_Single_Y_func_Area_(double A)
   :outertype: Ebes

Interpolation_I_Single_Y_func_Wxy_
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public double Interpolation_I_Single_Y_func_Wxy_(double Wxy)
   :outertype: Ebes

Interpolation_I_Single_Y_func_Wxz_
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public double Interpolation_I_Single_Y_func_Wxz_(double Wxz)
   :outertype: Ebes

Interpolation_I_Single_Z_func_Y_
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public double Interpolation_I_Single_Z_func_Y_(double Y)
   :outertype: Ebes

Interpolation_I_Single_ey_func_Y_
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public double Interpolation_I_Single_ey_func_Y_(double Y)
   :outertype: Ebes

Interpolation_I_Single_ez_func_Y_
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public double Interpolation_I_Single_ez_func_Y_(double Y)
   :outertype: Ebes

MatrixStiffness
^^^^^^^^^^^^^^^

.. java:method:: public double MatrixStiffness(int i)
   :outertype: Ebes

Straini
^^^^^^^

.. java:method:: public double Straini(int i, int element, int hypothesis)
   :outertype: Ebes

Variable_Position
^^^^^^^^^^^^^^^^^

.. java:method:: public int Variable_Position()
   :outertype: Ebes

createSolution
^^^^^^^^^^^^^^

.. java:method:: @Override public DoubleSolution createSolution()
   :outertype: Ebes

evaluate
^^^^^^^^

.. java:method:: @Override public void evaluate(DoubleSolution solution)
   :outertype: Ebes

   Evaluates a solution

   :param solution: The solution to evaluate

evaluateConstraints
^^^^^^^^^^^^^^^^^^^

.. java:method:: @Override public void evaluateConstraints(DoubleSolution solution)
   :outertype: Ebes

   Evaluates the constraint overhead of a solution

   :param solution: The solution
   :throws JMetalException:

geometryCheck
^^^^^^^^^^^^^

.. java:method:: public int geometryCheck(int i, int j)
   :outertype: Ebes

getElement
^^^^^^^^^^

.. java:method:: public double getElement(int i, int j)
   :outertype: Ebes

getElementsBetweenDiffGreat
^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public int getElementsBetweenDiffGreat()
   :outertype: Ebes

getGroupShape
^^^^^^^^^^^^^

.. java:method:: public int getGroupShape(int groupId)
   :outertype: Ebes

getGroups
^^^^^^^^^

.. java:method:: public double getGroups(int i)
   :outertype: Ebes

getMatrixWidthBand
^^^^^^^^^^^^^^^^^^

.. java:method:: public int getMatrixWidthBand()
   :outertype: Ebes

getMxyMax
^^^^^^^^^

.. java:method:: public double getMxyMax(int group, int hypothesis)
   :outertype: Ebes

getMxyMin
^^^^^^^^^

.. java:method:: public double getMxyMin(int group, int hypothesis)
   :outertype: Ebes

getMxzMax
^^^^^^^^^

.. java:method:: public double getMxzMax(int group, int hypothesis)
   :outertype: Ebes

getMxzMin
^^^^^^^^^

.. java:method:: public double getMxzMin(int group, int hypothesis)
   :outertype: Ebes

getNode
^^^^^^^

.. java:method:: public double getNode(int i, int j)
   :outertype: Ebes

getNodeRestrict
^^^^^^^^^^^^^^^

.. java:method:: public double getNodeRestrict(int i, int j)
   :outertype: Ebes

getNumberOfConstraintsNodes
^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public int getNumberOfConstraintsNodes()
   :outertype: Ebes

getNumberOfElements
^^^^^^^^^^^^^^^^^^^

.. java:method:: public int getNumberOfElements()
   :outertype: Ebes

getNumberOfNodes
^^^^^^^^^^^^^^^^

.. java:method:: public int getNumberOfNodes()
   :outertype: Ebes

getNumberOfNodesRestricts
^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public int getNumberOfNodesRestricts()
   :outertype: Ebes

getNumberOfWeigthHypothesis
^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public int getNumberOfWeigthHypothesis()
   :outertype: Ebes

getNumberOfWeigthsElements
^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public int getNumberOfWeigthsElements()
   :outertype: Ebes

getNumberOfWeigthsNodes
^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public int getNumberOfWeigthsNodes()
   :outertype: Ebes

getNxxMax
^^^^^^^^^

.. java:method:: public double getNxxMax(int group, int hypothesis)
   :outertype: Ebes

getNxxMin
^^^^^^^^^

.. java:method:: public double getNxxMin(int group, int hypothesis)
   :outertype: Ebes

getOldStrainMax
^^^^^^^^^^^^^^^

.. java:method:: public double getOldStrainMax(int group, int hypothesis)
   :outertype: Ebes

getOldStrainMin
^^^^^^^^^^^^^^^

.. java:method:: public double getOldStrainMin(int group, int hypothesis)
   :outertype: Ebes

getOmegaMax
^^^^^^^^^^^

.. java:method:: public double getOmegaMax(int group, int hypothesis)
   :outertype: Ebes

getStrainAdmissibleCut
^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public int getStrainAdmissibleCut()
   :outertype: Ebes

getStrainCutMax
^^^^^^^^^^^^^^^

.. java:method:: public double getStrainCutMax(int group, int hypothesis)
   :outertype: Ebes

getStrainMax
^^^^^^^^^^^^

.. java:method:: public double getStrainMax(int group, int hypothesis)
   :outertype: Ebes

getStrainMin
^^^^^^^^^^^^

.. java:method:: public double getStrainMin(int group, int hypothesis)
   :outertype: Ebes

getStrainMxyMax
^^^^^^^^^^^^^^^

.. java:method:: public double getStrainMxyMax(int group, int hypothesis)
   :outertype: Ebes

getStrainMxyMin
^^^^^^^^^^^^^^^

.. java:method:: public double getStrainMxyMin(int group, int hypothesis)
   :outertype: Ebes

getStrainMxzMax
^^^^^^^^^^^^^^^

.. java:method:: public double getStrainMxzMax(int group, int hypothesis)
   :outertype: Ebes

getStrainMxzMin
^^^^^^^^^^^^^^^

.. java:method:: public double getStrainMxzMin(int group, int hypothesis)
   :outertype: Ebes

getStrainNxxMax
^^^^^^^^^^^^^^^

.. java:method:: public double getStrainNxxMax(int group, int hypothesis)
   :outertype: Ebes

getStrainNxxMin
^^^^^^^^^^^^^^^

.. java:method:: public double getStrainNxxMin(int group, int hypothesis)
   :outertype: Ebes

getStrainResidualCut
^^^^^^^^^^^^^^^^^^^^

.. java:method:: public double getStrainResidualCut(int hypothesis)
   :outertype: Ebes

getStrainResidualMax
^^^^^^^^^^^^^^^^^^^^

.. java:method:: public double getStrainResidualMax(int hypothesis)
   :outertype: Ebes

getStrainResidualMin
^^^^^^^^^^^^^^^^^^^^

.. java:method:: public double getStrainResidualMin(int hypothesis)
   :outertype: Ebes

getStrainj
^^^^^^^^^^

.. java:method:: public double getStrainj(int i, int element, int hypothesis)
   :outertype: Ebes

getVariablePosition
^^^^^^^^^^^^^^^^^^^

.. java:method:: public int getVariablePosition(int groupId)
   :outertype: Ebes

getWeightElement
^^^^^^^^^^^^^^^^

.. java:method:: public double getWeightElement(int i, int j)
   :outertype: Ebes

getWeightElementItself
^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public double getWeightElementItself(int i, int j)
   :outertype: Ebes

getWeightNode
^^^^^^^^^^^^^

.. java:method:: public double getWeightNode(int i, int j)
   :outertype: Ebes

getnumberOfConstraintsGeometric
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public int getnumberOfConstraintsGeometric()
   :outertype: Ebes

getnumberOfGroupElements
^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public int getnumberOfGroupElements()
   :outertype: Ebes

nodeCheck
^^^^^^^^^

.. java:method:: public double nodeCheck(int i, int j)
   :outertype: Ebes

numberOfNodesRestricts
^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public void numberOfNodesRestricts(int numberOfNodesRestricts)
   :outertype: Ebes

setElementsBetweenDiffGreat
^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public void setElementsBetweenDiffGreat(int elementsBetweenDiffGreat)
   :outertype: Ebes

setMatrixWidthBand
^^^^^^^^^^^^^^^^^^

.. java:method:: public void setMatrixWidthBand(int matrixWidthBand)
   :outertype: Ebes

setNumberOfConstraintsNodes
^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public void setNumberOfConstraintsNodes(int numberOfConstraintsNodes)
   :outertype: Ebes

setNumberOfElements
^^^^^^^^^^^^^^^^^^^

.. java:method:: public void setNumberOfElements(int numberOfElements)
   :outertype: Ebes

setNumberOfNodes
^^^^^^^^^^^^^^^^

.. java:method:: public void setNumberOfNodes(int numberOfNodes)
   :outertype: Ebes

setNumberOfWeigthHypothesis
^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public void setNumberOfWeigthHypothesis(int numberOfWeigthHypothesis)
   :outertype: Ebes

setNumberOfWeigthsElements
^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public void setNumberOfWeigthsElements(int numberOfWeigthsElements)
   :outertype: Ebes

setNumberOfWeigthsNodes
^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public void setNumberOfWeigthsNodes(int numberOfWeigthsNodes)
   :outertype: Ebes

setStrainAdmissibleCut
^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public void setStrainAdmissibleCut(int strainAdmissibleCut)
   :outertype: Ebes

setnumberOfConstraintsGeometric
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public void setnumberOfConstraintsGeometric(int i)
   :outertype: Ebes

setnumberOfGroupElements
^^^^^^^^^^^^^^^^^^^^^^^^

.. java:method:: public void setnumberOfGroupElements(int i)
   :outertype: Ebes

