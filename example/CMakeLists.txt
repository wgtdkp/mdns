add_executable(mdns-example
    main.c
)

target_compile_options(mdns-example
    PRIVATE -Wno-unused-parameter
)

target_link_libraries(mdns-example
    PRIVATE mdns
)
