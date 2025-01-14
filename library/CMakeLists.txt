cmake_minimum_required(VERSION 3.10)

# Define the library target
add_library(MyLibrary library.cpp)

# Specify include directories
target_include_directories(MyLibrary PUBLIC ${CMAKE_CURRENT_SOURCE_DIR})