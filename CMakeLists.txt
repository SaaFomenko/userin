cmake_minimum_required(VERSION 3.5)

project(userin)

file(GLOB
	lib_source "*.cpp")

set(CMAKE_WINDOWS_EXPORT_ALL_SYMBOLS ON)
add_library(${PROJECT_NAME}_lib STATIC ${lib_source} ${rand_of_range})
