#
cmake_minimum_required(VERSION 3.25)

#
project(Template VERSION 1.0)

# Include Directories
target_include_directories(Tutorial PUBLIC "${PROJECT_BINARY_DIR}")

# Modify files from CMake
configure_file(templateConfig.h.in templateConfig.h)

#
set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED True)

#
add_executable(Template templateSource.cpp)

