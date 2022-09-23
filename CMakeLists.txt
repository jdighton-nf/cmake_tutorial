# Simple hello world
# The point of this is to set up a config, and to allow cmake to do all the work writing makefiles 

cmake_minimum_required(VERSION 3.10)    # minimum cmake required
set(CMAKE_CXX_STANDARD 17)              # C++ standard specs
set(CMAKE_CXX_STANDARD_REQUIRED ON)

project(hello VERSION 1.0)              # Give it a name
add_executable(hello main.cpp)          # Specify what to call executable, and what is the entry point 
target_include_directories(hello PUBLIC ${CMAKE_CURRENT_SOURCE_DIR/include})

