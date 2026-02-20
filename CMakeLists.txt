cmake_minimum_required(VERSION 3.16)
project(terrain_walker LANGUAGES C CXX)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

add_library(glad STATIC
	external/glad/src/glad.c
)

target_include_directories(glad PUBLIC
	external/glad/include
)

find_package(glfw3 REQUIRED)
find_package(OpenGL REQUIRED)

add_executable(terrain_walker
	src/main.cpp
)

target_link_libraries(terrain_walker
	glad
	glfw
	OpenGL::GL
)
