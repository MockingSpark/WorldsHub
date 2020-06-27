
file(GLOB SOURCES_MAIN CONFIGURE_DEPENDS */*.h */*.cpp WHub.cpp)
file(GLOB SOURCES_TEST CONFIGURE_DEPENDS */*.h */*.cpp test.cpp)

add_executable(WorldsHub
  ${SOURCES_MAIN}
  )

target_link_libraries(WorldsHub PUBLIC sfml-graphics)

add_executable(TestHub
        ${SOURCES_TEST}
        )

target_link_libraries(TestHub PUBLIC sfml-graphics)