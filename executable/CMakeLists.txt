project(MyCppProject)

cmake_minimum_required(VERSION 3.10)

set(CMAKE_CXX_STANDARD 11)

# Specify the source files for the executable
set(SOURCES
    main.cpp
)

# Add the executable target
add_executable(MyExecutable ${SOURCES})

# Include directories for the executable
target_include_directories(MyExecutable PRIVATE ${CMAKE_SOURCE_DIR}/library)

# Link the executable with the library
target_link_libraries(MyExecutable PRIVATE MyLibrary)