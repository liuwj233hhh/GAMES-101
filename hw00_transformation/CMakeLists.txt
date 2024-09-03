cmake_minimum_required (VERSION 3.30.3)
project (hw0_transformation)

find_package(Eigen3 REQUIRED)
include_directories("/usr/local/include")

add_executable (main main.cpp)