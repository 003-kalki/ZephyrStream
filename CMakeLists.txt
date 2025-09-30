cmake_minimum_required(VERSION 3.10)

# Project name and version
project(DistributedQueue VERSION 1.0 LANGUAGES CXX)

# Set C++ standard
set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED True)

# Include directories
include_directories(include)

# Source files
file(GLOB_RECURSE SOURCES src/*.cpp)

# Create executable
add_executable(my_kafka ${SOURCES})

# Optional: link libraries if needed
# target_link_libraries(my_kafka <library_name>)
