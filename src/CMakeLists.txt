add_library(mdns
    mdns.c
)

target_include_directories(mdns
    PUBLIC ${PROJECT_SOURCE_DIR}/include
)
