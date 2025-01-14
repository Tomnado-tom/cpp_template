# Set the minimum required version of CMake
cmake_minimum_required(VERSION 3.10)

add_subdirectory(googletest)
set_target_properties(gmock PROPERTIES FOLDER "Vendor/Test")
set_target_properties(gmock_main PROPERTIES FOLDER "Vendor/Test")
set_target_properties(gtest PROPERTIES FOLDER "Vendor/Test")
set_target_properties(gtest_main PROPERTIES FOLDER "Vendor/Test")
