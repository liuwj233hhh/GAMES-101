cmake_minimum_required(VERSION 3.30.3)
project(hw01_rotation_projection)

find_package(OpenCV 4 REQUIRED)

set(CMAKE_CXX_STANDARD 17)

message(STATUS "OpenCV version: ${OpenCV_VERSION}")

include_directories("/usr/local/include")
include_directories( ${OpenCV_INCLUDE_DIRS} )

add_executable(Rasterizer main.cpp rasterizer.hpp rasterizer.cpp Triangle.hpp Triangle.cpp)
target_link_libraries(Rasterizer ${OpenCV_LIBRARIES})
