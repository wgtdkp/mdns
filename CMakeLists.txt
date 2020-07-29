cmake_minimum_required(VERSION 3.10.0)
project(mdns LANGUAGES C)

option(MDNS_EXAMPLE "Build mDNS example" ON)

if (NOT CMAKE_BUILD_TYPE)
    set(CMAKE_BUILD_TYPE Release)
endif()

# Global compilation options for libraries and executables.
add_compile_options(
    -Wall
    -Wextra
    -Wpedantic
    -Werror
    -Wfatal-errors
)

add_subdirectory(src)
add_subdirectory(example)
