project(tests)

# Specify the C++ standard
set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED True)

# Include the Google Test framework
enable_testing()
find_package(GTest REQUIRED)
include_directories(${GTEST_INCLUDE_DIRS})

# Add the test executable
add_executable(tests test_main.cpp)

# Link the test executable with the Google Test libraries
target_link_libraries(tests ${GTEST_LIBRARIES} pthread)

# Add the test cases
add_test(NAME MyTests COMMAND tests)