cmake_minimum_required(VERSION 3.15)
cmake_policy(VERSION 3.15)

include(FetchContent)
project(JIN4 VERSION 1.0.0 LANGUAGES CXX)

set (BUILD_SHARED_LIBS FALSE)

FetchContent_Declare(
    sfml
    GIT_REPOSITORY https://github.com/SFML/SFML.git
    GIT_TAG 2.5.1
)

FetchContent_MakeAvailable(sfml)

add_subdirectory(src)

