add_library(instantiation_lib SHARED instantiation.cpp)
target_include_directories(instantiation_lib PUBLIC ${CMAKE_SOURCE_DIR})
