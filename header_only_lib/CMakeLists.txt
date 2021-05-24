CMAKE_MINIMUM_REQUIRED(VERSION 3.5)

project(header_only_test)
add_library(lib INTERFACE)
#target_sources(lib INTERFACE greeting.hpp)
target_include_directories(lib INTERFACE include)
set_target_properties(lib PROPERTIES LINKER_LANGUAGE CXX)

add_executable(test test/test.cpp)
target_include_directories(test PRIVATE include)
target_link_libraries(test PRIVATE lib)