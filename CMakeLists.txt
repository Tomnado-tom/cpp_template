project(my_cpp_project)

cmake_minimum_required(VERSION 3.10)

# Include subdirectories
add_subdirectory(executable)
add_subdirectory(library)
add_subdirectory(tests)
add_subdirectory(vendor)