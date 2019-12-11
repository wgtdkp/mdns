set(TARGET_NAME mdns-test)

set(SRCS main.c)

add_executable(${TARGET_NAME} ${SRCS})
target_link_libraries(${TARGET_NAME} mdns)
