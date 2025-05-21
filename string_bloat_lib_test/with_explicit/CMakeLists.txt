cmake_minimum_required(VERSION 3.16)
project(string_bloat_minimal_shared_lib_test)

set(CMAKE_CXX_STANDARD 20)
add_subdirectory(instantiation_lib)

add_executable(bloat_test main.cpp)
target_include_directories(bloat_test PRIVATE ${CMAKE_SOURCE_DIR})
target_link_libraries(bloat_test PRIVATE instantiation_lib)
