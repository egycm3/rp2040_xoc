cmake_minimum_required(VERSION 3.12)

include(pico_sdk_import.cmake)

project(rp2040_xoc C CXX ASM)
set(CMAKE_C_STANDARD 11)
set(CMAKE_CXX_STANDARD 17)

# Initialize the SDK
pico_sdk_init()

# Hardware-specific examples in subdirectories:
add_subdirectory(clock_stat)
add_subdirectory(XOC)
add_subdirectory(dhry)
add_subdirectory(XOC_dhry)