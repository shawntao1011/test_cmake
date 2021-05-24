add_executable(test sample.cpp)
target_include_directories(test PRIVATE ../include)
target_link_libraries(test PRIVATE lib)