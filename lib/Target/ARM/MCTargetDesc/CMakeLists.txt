add_llvm_library(LLVMARMDesc
  ARMAsmBackend.cpp
  ARMMCTargetDesc.cpp
  ARMMCAsmInfo.cpp
  ARMMCCodeEmitter.cpp
  ARMMCExpr.cpp
  ARMMachObjectWriter.cpp
  )

# Hack: we need to include 'main' target directory to grab private headers
include_directories(${CMAKE_CURRENT_SOURCE_DIR}/.. ${CMAKE_CURRENT_BINARY_DIR}/..)
