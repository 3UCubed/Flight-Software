####
# F prime CMakeLists.txt:
#
# SOURCE_FILES: combined list of source and autocoding diles
# MOD_DEPS: (optional) module dependencies
#
# Note: using PROJECT_NAME as EXECUTABLE_NAME
####
set(SOURCE_FILES
  "${CMAKE_CURRENT_LIST_DIR}/STM32BlinkTopologyAppAi.xml"
  "${CMAKE_CURRENT_LIST_DIR}/Topology.cpp"  
  "${CMAKE_CURRENT_LIST_DIR}/Main.cpp"  
)
# Note: supply non-explicit dependencies here
set(MOD_DEPS
  Fw/Logger
  Svc/RTOSTime
  # Communication Implementations
)
register_fprime_executable()
