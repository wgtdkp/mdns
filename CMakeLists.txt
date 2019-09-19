project(mdns C)
cmake_minimum_required(VERSION 3.0.2)

set(CMAKE_BUILD_TYPE Release)
set(CMAKE_C_FLAGS "-std=c11 -Wall -Werror -Wfatal-errors")

set(TARGET_NAME mdns)

set(SRCS mdns.c)
add_library(${TARGET_NAME} STATIC ${SRCS})
add_executable(mdns-test main.c)
target_link_libraries(mdns-test ${TARGET_NAME})
