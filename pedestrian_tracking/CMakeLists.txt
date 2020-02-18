cmake_minimum_required(VERSION 3.0 FATAL_ERROR)

add_definitions(-std=c++11)

set(CXX_FLAGS "-Wall")
set(CMAKE_CXX_FLAGS, "${CXX_FLAGS}")

find_package(PkgConfig)
pkg_search_module(Eigen3 REQUIRED eigen3)

add_executable(test_script src/test.cpp)
