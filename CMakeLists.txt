cmake_minimum_required(VERSION 3.13.1)
project(mdns LANGUAGES C)

if (NOT CMAKE_BUILD_TYPE)
    set(CMAKE_BUILD_TYPE Release)
endif()

# TODO(wgtdkp): kill CMAKE_XXX_FLAGS
set(CMAKE_C_FLAGS "-std=gnu11 -Wall -Werror -Wfatal-errors")

add_subdirectory(src)
add_subdirectory(tests)
