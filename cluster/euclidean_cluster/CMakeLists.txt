cmake_minimum_required(VERSION 2.8 FATAL_ERROR)

project(euclidean_cluster)
 
find_package(PCL 1.8 REQUIRED)
 
include_directories(${PCL_INCLUDE_DIRS})
link_directories(${PCL_LIBRARY_DIRS})
add_definitions(${PCL_DEFINITIONS})
 
add_executable(euclidean_cluster euclidean_cluster.cc)
target_link_libraries (euclidean_cluster ${PCL_LIBRARIES})