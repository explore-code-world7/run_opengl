cmake_minimum_required(VERSION 2.8.1)

project(window)

find_package(glfw3 REQUIRED)
add_library(glad 3rdparty/glad/src/glad.c)

add_executable(window window.cpp)

target_link_libraries(window  glfw  glad)
