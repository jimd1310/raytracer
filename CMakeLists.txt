cmake_minimum_required(VERSION 3.20)

project(raytracer LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

add_executable(raytracer main.cc)

target_include_directories(raytracer PRIVATE
    ${PROJECT_SOURCE_DIR}/include
)

target_compile_options(raytracer PRIVATE
    -Wall -Wextra -Wpedantic
)