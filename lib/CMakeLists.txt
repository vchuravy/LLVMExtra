llvm_add_library(
  LLVMExtra
  SHARED
  llvm-api.cpp
  LINK_LIBS PRIVATE
  LLVM
  ${LLVM_PTHREAD_LIB}
)
llvm_update_compile_flags(LLVMExtra)
