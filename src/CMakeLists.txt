add_library(mdns)

target_sources(mdns
    PRIVATE mdns.c
)

target_include_directories(mdns
    PUBLIC ${PROJECT_SOURCE_DIR}/include
)
