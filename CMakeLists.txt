cmake_minimum_required(VERSION 3.0.0)

project(glew VERSION 2.1.0)

set(CMAKE_CXX_STANDARD 11)
set(CMAKE_C_STANDARD 11)

add_definitions(-DGLEW_STATIC)
add_definitions(-DGLEW_NO_GLU)

include_directories(${CMAKE_CURRENT_SOURCE_DIR}/include/)

add_library(${PROJECT_NAME} STATIC ${CMAKE_CURRENT_SOURCE_DIR}/src/glew.c)