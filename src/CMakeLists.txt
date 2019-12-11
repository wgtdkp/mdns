set(TARGET_NAME mdns)

set(SRCS mdns.c)

add_library(${TARGET_NAME} STATIC ${SRCS})
target_include_directories(${TARGET_NAME} PUBLIC ${PROJECT_SOURCE_DIR}/include)
