cmake_minimum_required(VERSION 3.10)

project(smuduo)

set(CMAKE_CXX_STANDARD 11)

# Collect all source files
file(GLOB_RECURSE SOURCES "*.cc")

# Create a shared library
add_library(smuduo SHARED ${SOURCES})

# Link any necessary libraries
target_link_libraries(smuduo pthread)
