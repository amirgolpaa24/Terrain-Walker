# Terrain Walker

Terrain Walker is a C++ OpenGL project for rendering and exploring procedurally generated terrain in first-person view.

The goal is to build a real-time terrain engine step by step, starting from a simple heightmap renderer and evolving toward a dynamic, infinite world system.

## Tech Stack

- C++
- OpenGL (Core Profile)
- GLFW
- GLAD
- GLM
- CMake

## Build

```bash
cmake -S . -B build
cmake --build build
./build/terrain_walker
