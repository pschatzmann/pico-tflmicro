
cmake_minimum_required(VERSION 3.12)

# Pull in PICO SDK (must be before project)
include(pico_sdk_import.cmake)

project(pico-tflmicro-all C CXX ASM)
set(CMAKE_C_STANDARD 11)
set(CMAKE_CXX_STANDARD 11)

pico_sdk_init()

add_subdirectory("src")
add_subdirectory("examples" EXCLUDE_FROM_ALL)
add_subdirectory("tests" EXCLUDE_FROM_ALL)
