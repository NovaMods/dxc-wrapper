

# ===============================================
# configure executable

file(GLOB_RECURSE SOURCES "src/*.cc" "src/*.hh")
arcana_source_group(SOURCES)

add_executable(dxc-wrapper-standalone ${SOURCES})
target_include_directories(dxc-wrapper-standalone PUBLIC src/)
target_link_libraries(dxc-wrapper-standalone PUBLIC dxc-wrapper)
