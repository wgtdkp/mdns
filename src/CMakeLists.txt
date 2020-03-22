add_library(mdns mdns.c)
target_compile_features(mdns PUBLIC c_std_11)
target_include_directories(mdns PUBLIC ${PROJECT_SOURCE_DIR}/include)
