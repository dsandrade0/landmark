cmake_minimum_required (VERSION 2.6)
project (face)
find_package (OpenCV 3.4.2 REQUIRED)
include_directories( ${OpenCV_INCLUDE_DIRS} )
add_executable (face src/facialLandmarkDetection.cpp)
target_link_libraries( face ${OpenCV_LIBS} )
