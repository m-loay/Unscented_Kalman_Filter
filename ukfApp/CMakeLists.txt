# set minimum cmake version
cmake_minimum_required(VERSION 2.8.9 FATAL_ERROR)

# project name and language
project(ukfApp)

#set standard of C++11 and build type to debug
set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED True)
set(CMAKE_BUILD_TYPE Debug)

include_directories ("${KCONFIG_INCLIDE_DIR}")
include_directories ("${KFLIB_INCLIDE_DIR}")
add_library(ukfApp STATIC ukfApp.cpp)
