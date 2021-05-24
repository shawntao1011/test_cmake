CMAKE_MINIMUM_REQUIRED(VERSION 3.5)

add_library(mylib STATIC source/add.cpp)

target_include_directories(mylib PRIVATE header)


