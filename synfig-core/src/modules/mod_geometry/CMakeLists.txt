add_library(mod_geometry MODULE "")

target_sources(mod_geometry
    PUBLIC
        "${CMAKE_CURRENT_LIST_DIR}/advanced_outline.cpp"
        "${CMAKE_CURRENT_LIST_DIR}/checkerboard.cpp"
        "${CMAKE_CURRENT_LIST_DIR}/circle.cpp"
        "${CMAKE_CURRENT_LIST_DIR}/main.cpp"
        "${CMAKE_CURRENT_LIST_DIR}/outline.cpp"
        "${CMAKE_CURRENT_LIST_DIR}/rectangle.cpp"
        "${CMAKE_CURRENT_LIST_DIR}/region.cpp"
        "${CMAKE_CURRENT_LIST_DIR}/star.cpp"
)

install (
    TARGETS mod_geometry
    DESTINATION lib/synfig/modules
)
