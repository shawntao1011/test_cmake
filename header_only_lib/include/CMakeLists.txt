add_library(lib INTERFACE)
#target_sources(lib INTERFACE greeting.hpp)
target_include_directories(lib INTERFACE .)
set_target_properties(lib PROPERTIES LINKER_LANGUAGE CXX)