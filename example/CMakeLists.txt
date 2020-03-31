add_executable(mdns-example)

target_sources(mdns-example
    PRIVATE main.c
)

target_compile_options(mdns-example
    PRIVATE -Wno-unused-parameter
)

target_link_libraries(mdns-example
    PRIVATE mdns
)
