cmake_minimum_required(VERSION 3.26)
project(temp)

set(CMAKE_CXX_STANDARD 23)

find_package(OpenGL REQUIRED)

add_executable(temp
        src/glad.h
        src/glad.c
        src/main.cpp
)

target_link_libraries(temp glfw OpenGL::GL)