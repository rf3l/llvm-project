# Exclude tests from libMLIR.so
add_mlir_library(MLIRLinalgTestPasses
  TestLinalgCodegenStrategy.cpp
  TestLinalgElementwiseFusion.cpp
  TestLinalgFusionTransforms.cpp
  TestLinalgHoisting.cpp
  TestLinalgTransforms.cpp
  TestPadFusion.cpp

  EXCLUDE_FROM_LIBMLIR

  LINK_LIBS PUBLIC
  MLIRAffine
  MLIRAffineBufferizableOpInterfaceImpl
  MLIRArithmetic
  MLIRArithmeticTransforms
  MLIRBufferization
  MLIRBufferizationTransforms
  MLIRGPUTransforms
  MLIRLinalg
  MLIRLinalgTransforms
  MLIRLLVMToLLVMIRTranslation
  MLIRMemRef
  MLIRPass
  MLIRSCF
  MLIRSCFTransforms
  MLIRTensor
  MLIRTensorTransforms
  MLIRTransformUtils
  MLIRVector
  MLIRVectorToSCF
  MLIRVectorTransforms
  )
